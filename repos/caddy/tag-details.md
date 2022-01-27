<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
-	[`caddy:2.4.6`](#caddy246)
-	[`caddy:2.4.6-alpine`](#caddy246-alpine)
-	[`caddy:2.4.6-builder`](#caddy246-builder)
-	[`caddy:2.4.6-builder-alpine`](#caddy246-builder-alpine)
-	[`caddy:2.4.6-builder-windowsservercore-1809`](#caddy246-builder-windowsservercore-1809)
-	[`caddy:2.4.6-builder-windowsservercore-ltsc2016`](#caddy246-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.6-windowsservercore`](#caddy246-windowsservercore)
-	[`caddy:2.4.6-windowsservercore-1809`](#caddy246-windowsservercore-1809)
-	[`caddy:2.4.6-windowsservercore-ltsc2016`](#caddy246-windowsservercore-ltsc2016)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2016`](#caddybuilder-windowsservercore-ltsc2016)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2016`](#caddywindowsservercore-ltsc2016)

## `caddy:2`

```console
$ docker pull caddy@sha256:af86498f48007129b4656236533520811fba83b2dd25e9e6f5ac5d59a4639f44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:1659785ea84188c3ad22a6c1f96f463d167a4b81318d71f4bb6e3d37dbe73908
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
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:28e1e2e65edbfd6d151a56bcaac22e8d8fe9deb1f5855db6e0a7aa51db9d580b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4886; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:5bbea3c4df3d7c544eed70812f8cf2939e1b45d8fd8de5cbee96f4d0d2b654ae
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
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89b3dac80f3f9c2cfa6a51201d66a6ce07cc824ab9c160cc9529794802ddcd61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a6a37a033e28b11743049e8fc620b798a4e8fda291740c376b869184ff77954e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:70079683faad29699732179ae14ebd3ad2ef8330645ef775f581cf555496e15a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f504e734712cf31dc0903f54de87aa8791a825b7894d33a007da91b42a178a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9f877e9983e295396f9d05504d82d70c7d34027e8fc2c3d86861ebec4932df59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4889; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6`

```console
$ docker pull caddy@sha256:af86498f48007129b4656236533520811fba83b2dd25e9e6f5ac5d59a4639f44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:2.4.6` - linux; amd64

```console
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-alpine`

```console
$ docker pull caddy@sha256:1659785ea84188c3ad22a6c1f96f463d167a4b81318d71f4bb6e3d37dbe73908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.6-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder`

```console
$ docker pull caddy@sha256:28e1e2e65edbfd6d151a56bcaac22e8d8fe9deb1f5855db6e0a7aa51db9d580b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4886; amd64

### `caddy:2.4.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-alpine`

```console
$ docker pull caddy@sha256:5bbea3c4df3d7c544eed70812f8cf2939e1b45d8fd8de5cbee96f4d0d2b654ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.6-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89b3dac80f3f9c2cfa6a51201d66a6ce07cc824ab9c160cc9529794802ddcd61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2.4.6-builder-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a6a37a033e28b11743049e8fc620b798a4e8fda291740c376b869184ff77954e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `caddy:2.4.6-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore`

```console
$ docker pull caddy@sha256:70079683faad29699732179ae14ebd3ad2ef8330645ef775f581cf555496e15a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:2.4.6-windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-windowsservercore` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:f504e734712cf31dc0903f54de87aa8791a825b7894d33a007da91b42a178a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:2.4.6-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9f877e9983e295396f9d05504d82d70c7d34027e8fc2c3d86861ebec4932df59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4889; amd64

### `caddy:2.4.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:1659785ea84188c3ad22a6c1f96f463d167a4b81318d71f4bb6e3d37dbe73908
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
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:28e1e2e65edbfd6d151a56bcaac22e8d8fe9deb1f5855db6e0a7aa51db9d580b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4886; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:5bbea3c4df3d7c544eed70812f8cf2939e1b45d8fd8de5cbee96f4d0d2b654ae
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
$ docker pull caddy@sha256:010009b3178957f4c616f675a5e7f88e1b63333fd51418f37d356580d177db41
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121310128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dfe8eb81a78669ea112df14a2aad3c4e1a6e85e97f863a44b9fb467389fb2bb1`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:21:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:21:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:21:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:21:15 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:23:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:23:25 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:23:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:23:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:23:26 GMT
WORKDIR /go
# Thu, 06 Jan 2022 22:52:44 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 22:52:44 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 22:52:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 22:52:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 22:52:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 22:52:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666ba61612fd7c93393f9a5bc1751d8a9929e32d51501dba691da9e8232bc87b`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 282.2 KB (282159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed8ca4862056a130f714accb3538decfa0663fec84e635d8b5a0a3305353dee`  
		Last Modified: Tue, 30 Nov 2021 04:36:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe6c5a15a65f4960a2b1852b3f3221cfb89fccf18b6125213d9c40143a20b80`  
		Last Modified: Thu, 06 Jan 2022 22:33:56 GMT  
		Size: 110.1 MB (110142583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a0e8bec74ddb73c81aa4e49168ff2ca80c701bd2d6e66a7124a70344f35961`  
		Last Modified: Thu, 06 Jan 2022 22:33:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6b9a9093087dda6ca0b3706ad12ea1e4f3eecc5906caa25ddb2081a89b6e6e`  
		Last Modified: Thu, 06 Jan 2022 22:53:07 GMT  
		Size: 6.8 MB (6821284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c8f22ae2a46690d2716974c8992ee21be6007cd51846e848d79abb9c9568e`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 1.2 MB (1244975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5c2bdf23d4163ce8187d4bef992720d3ab9e49da5c1177c0859887ca7ab460`  
		Last Modified: Thu, 06 Jan 2022 22:53:05 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:61c53db5e73a02ef8f2d7768520fdc8b6512bf685bec9b2765c108043efe30db
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115770894 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb33b243903e47c65c3077fda209832aacb6774b0aede014e4cc40d460b52cfa`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:32:18 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 02:32:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 02:32:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:50:05 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:53:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:53:43 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:53:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:53:45 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:53:46 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:28:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:28:06 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:28:06 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:28:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:28:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:28:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:28:10 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228ad0256439cce3fe9db355991b0557f55241d8cca8690f4f741e1c2d8fb8b9`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 282.1 KB (282105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cab2a064767512d7d354e806cbd8b24ffefc15e06eeb7d4b127e7f6cddb6b40`  
		Last Modified: Tue, 30 Nov 2021 02:47:28 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa3eff05a8e767c828ccba11dafcaa949f5135fb474501562c760104485d17c7`  
		Last Modified: Thu, 06 Jan 2022 23:07:26 GMT  
		Size: 105.0 MB (105001999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a000d0fc1d42c7c9b7b860d6d172731f53e095440cd96a9b7c342be45ec9b08`  
		Last Modified: Thu, 06 Jan 2022 23:06:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0337bac10777aa11d25058ea3560262ee6db6fcfdc160e06ffb22f4c5fa1e9a8`  
		Last Modified: Thu, 06 Jan 2022 23:29:18 GMT  
		Size: 6.7 MB (6677078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a97361b5fa836384cffcbde78a2f88c65925e6f5e570b504691d61660a4249`  
		Last Modified: Thu, 06 Jan 2022 23:29:15 GMT  
		Size: 1.2 MB (1177576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fee5749cddc4c07f573e8c9fc686888f8317b076ec85df778cd4fe70022f7c5`  
		Last Modified: Thu, 06 Jan 2022 23:29:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:efbdb46b795bfc086fdd3dc3f083853144fee09f5f69cee30aad1042d951055d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114636784 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f24cb0ea441d11c66338d56d84d12ec2040db452771cf3239ac8cc58ade2894`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:10:37 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:10:39 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:10:39 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:16:55 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 23:20:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 23:20:10 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 23:20:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 23:20:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 23:20:13 GMT
WORKDIR /go
# Fri, 07 Jan 2022 00:07:55 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Jan 2022 00:07:55 GMT
ENV XCADDY_VERSION=v0.2.0
# Fri, 07 Jan 2022 00:07:56 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 07 Jan 2022 00:07:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 Jan 2022 00:07:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 Jan 2022 00:07:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 Jan 2022 00:07:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94f21e2af73375430a6481f93a61f3df4f9de38c985f83b27293f8aace16d6b5`  
		Last Modified: Tue, 30 Nov 2021 04:33:33 GMT  
		Size: 281.2 KB (281248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23cec97f9b59f8579851b3f2c1523c8a96065c591f5961858420e92bf9d424d2`  
		Last Modified: Tue, 30 Nov 2021 04:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7e10d2ccbec6995e3c5e0e1466b299b6772129bdfe2a7c9cd2de121fcd62372`  
		Last Modified: Thu, 06 Jan 2022 23:43:25 GMT  
		Size: 104.8 MB (104792199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bc7571575769c41c088a4855dec67f2298fbfc127d0b6fe27a11714a2ff85c`  
		Last Modified: Thu, 06 Jan 2022 23:42:17 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada6b849dbf6aa4efe75ed7d152710104c2efc1776722ae1ebf32e73e879a980`  
		Last Modified: Fri, 07 Jan 2022 00:09:08 GMT  
		Size: 6.0 MB (5951599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad12fa50847e7bce5e6320a80bd7cf7a7845053fbbbec10672fa9613997c41ef`  
		Last Modified: Fri, 07 Jan 2022 00:09:06 GMT  
		Size: 1.2 MB (1176261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8296185446e930a88732287bf9faf072335ccb581355255affc88c3f359be3e0`  
		Last Modified: Fri, 07 Jan 2022 00:09:05 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:d3578516d88bd737548a4dbc34d1f62d9ae221025593a5c109bf818b3521ddb8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3944d7f732293f6e32d4e7ffa7f34a2c1e4c7f59a17e712f4c7c868d308f6928`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 01:54:59 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 01:55:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 01:55:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:41:39 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:42:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:42:59 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:43:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:01 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:43:02 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:11:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:11:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:11:37 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:11:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:11:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:11:42 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:11:42 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a89e8eeedd549875510e5e4e14010906a58878526814e6df25d14009856c6ff`  
		Last Modified: Tue, 30 Nov 2021 02:05:10 GMT  
		Size: 281.9 KB (281899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94645a83ff95687e6f078c140cfcac8def006923ed4019ef74fa189e6d9f0b14`  
		Last Modified: Tue, 30 Nov 2021 02:05:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3a8bcf1eabba76537bfe5e366464a1b0945685149b09bfd0be21674035efdb`  
		Last Modified: Thu, 06 Jan 2022 22:52:52 GMT  
		Size: 104.4 MB (104371783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c92f367c5e773df00e89143be1b98a66727e464d2b3486747607d3cfd447f21`  
		Last Modified: Thu, 06 Jan 2022 22:52:37 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d036527718ca088f4cccf42b11f44f84f803586aebf32648678af9e7d4bd4f7`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 6.9 MB (6925777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea4ab2cf5eefe18e771b6b373cf0dfbac144754a4c2e88b3077b12eebeddd991`  
		Last Modified: Thu, 06 Jan 2022 23:12:13 GMT  
		Size: 1.1 MB (1148127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2579d0143e0a32e8389ea34deb661609463b24c04c60bff3f7b90aad159a4c0`  
		Last Modified: Thu, 06 Jan 2022 23:12:12 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:10c301564a8970c96a99e0986dcc07c2531e0a22ee9b515d078369230aa8b21c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114282804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:365a7415f1641e5937f47ac25abd2db349257cb1f410218076e09428cc2d8a57`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:17:54 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 03:17:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 03:18:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:33:50 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:36:06 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:36:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:36:15 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:36:17 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:07:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:07:02 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:07:04 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:07:11 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:07:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:07:15 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28be42a6852cc2108ddba1e4252671ae20275780a6ff73b1038699f59da2ac20`  
		Last Modified: Tue, 30 Nov 2021 03:35:16 GMT  
		Size: 284.0 KB (284020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d744d6799a13f2f7a7f85e040ddf0cc8b671a7cc5572b7049c3e1da8139b349`  
		Last Modified: Tue, 30 Nov 2021 03:35:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6b57588091597745a960477da30317e116ef20e2d738afebb226d12fac116b`  
		Last Modified: Thu, 06 Jan 2022 22:48:10 GMT  
		Size: 102.7 MB (102742856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c99ddb00388caae237e09e2b6eefcafadf60d1401cca689c3168ce0418bce118`  
		Last Modified: Thu, 06 Jan 2022 22:47:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d057dcb20cb5953109437e43d575a46411554b8e101a4897a55b19cfe35c35`  
		Last Modified: Thu, 06 Jan 2022 23:07:48 GMT  
		Size: 7.3 MB (7320426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176a9159fc9446ad5639d24776b14a32f716a5e62db5fff1780ec97834e4daf9`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 1.1 MB (1120009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba3cd4d1cf629a78023545daac45165694ebc0b0d0bf99c6f373f4e250b13bb`  
		Last Modified: Thu, 06 Jan 2022 23:07:47 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:b2bf3066a64ff8769975b2455f86d7e6b92d7ba2db6dc6ac2e8c27b1a99e4154
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118695222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33024957508086112d8f9d0dd4569e40d37d001c59ae2dfa128e5537c5047b7b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:07:57 GMT
RUN apk add --no-cache ca-certificates
# Tue, 30 Nov 2021 04:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Nov 2021 04:07:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:43:20 GMT
ENV GOLANG_VERSION=1.17.6
# Thu, 06 Jan 2022 22:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.6.src.tar.gz'; 		sha256='4dc1bbf3ff61f0c1ff2b19355e6d88151a70126268a47c761477686ef94748c8'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 06 Jan 2022 22:45:02 GMT
ENV GOPATH=/go
# Thu, 06 Jan 2022 22:45:02 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Jan 2022 22:45:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Jan 2022 22:45:03 GMT
WORKDIR /go
# Thu, 06 Jan 2022 23:12:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 06 Jan 2022 23:12:20 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 06 Jan 2022 23:12:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 Jan 2022 23:12:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 Jan 2022 23:12:21 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 Jan 2022 23:12:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66787da5af638f8523e4694d81d38c2ca7c0a262f4cb8d78c46f7d64833bbaa0`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 282.4 KB (282378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406f41068af489d7950f1a75d72455e702ed7da98dad21d9267448257b6a2ddc`  
		Last Modified: Tue, 30 Nov 2021 04:17:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d60e40a1edbdb9810c9bb4d0cff3698c895e5d6c4be23d2aa8fabdc3ab7d7c6`  
		Last Modified: Thu, 06 Jan 2022 22:54:34 GMT  
		Size: 107.7 MB (107672064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c510a70c425d2e9120d80be4dd15eb5b54bbc18b2d654979cf7cce6fd798ffbb`  
		Last Modified: Thu, 06 Jan 2022 22:54:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6066c32c506c543f8a0b0702e2fb744ad9ed66ebb2b1f9ab0143e16ddf0d2ddf`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 6.9 MB (6930614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c04b273d01906975a3ee8f1bbd75704d117639b00f402c6a4a0f83fd7c509`  
		Last Modified: Thu, 06 Jan 2022 23:12:56 GMT  
		Size: 1.2 MB (1203509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d12637b101d5162703ad7868f497c96bf15281a9369c82e54e8c589cb031c`  
		Last Modified: Thu, 06 Jan 2022 23:12:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:89b3dac80f3f9c2cfa6a51201d66a6ce07cc824ab9c160cc9529794802ddcd61
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:72af0e06b32a67c1a6bfa9204d4f2c702aed93b21813fae661fdfffdf554b680
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2886236941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f985de62284201d13a9b844cf326330406053348fdd15ae97730c4daa3b6b3ec`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 15:09:40 GMT
ENV GIT_VERSION=2.23.0
# Wed, 26 Jan 2022 15:09:41 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 26 Jan 2022 15:09:42 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 26 Jan 2022 15:09:43 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 26 Jan 2022 15:11:28 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:11:29 GMT
ENV GOPATH=C:\go
# Wed, 26 Jan 2022 15:12:29 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Jan 2022 15:29:08 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 26 Jan 2022 15:33:30 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Jan 2022 15:33:32 GMT
WORKDIR C:\go
# Wed, 26 Jan 2022 21:02:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:02:42 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 26 Jan 2022 21:02:43 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:02:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 26 Jan 2022 21:03:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 26 Jan 2022 21:03:56 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e066feb335981c422e18ec3e99d79f1c5be6b43ca35ab0430187cde79a8ba19`  
		Last Modified: Wed, 26 Jan 2022 16:03:50 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98ce4c8c854279fe1e91c71aa96b5228b24e217162fdc7508fa1ffed2d93f3e`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff64477d4a2364cc1faf09a8f6ca0359be8089d74617888efc97fc1ec2ec925`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5730c3ddd3a11e217b2bc0dd3198cefbc720787b51b86f921a046fb40be043a7`  
		Last Modified: Wed, 26 Jan 2022 16:03:47 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f86077710bb19cc328ec7f872e5557f814c2d3be829a2c1975471547f3adc7`  
		Last Modified: Wed, 26 Jan 2022 16:04:30 GMT  
		Size: 25.5 MB (25472102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01031350b313b8d7dc8b649f435561b95b072ded45bcb1e12d170b2d802406c1`  
		Last Modified: Wed, 26 Jan 2022 16:03:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8558cedae20f4e01a76f91a8787b6ffec7812eb6b0013980e19c208f3e7b0cf`  
		Last Modified: Wed, 26 Jan 2022 16:03:45 GMT  
		Size: 335.0 KB (335017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7f568a047da2280936ebaab2fd0479b3a6a5e9afa603fa8eba6f3fa1cc96d2`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db36d4d0813c6743a4407bdba7a0be0025b10f8cbedde63043409911b556d56`  
		Last Modified: Wed, 26 Jan 2022 16:16:20 GMT  
		Size: 145.4 MB (145423291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f910516d12aa2decb0589c60b2bc4f4400ff2edac20fd2377ab1ed892a5b6c65`  
		Last Modified: Wed, 26 Jan 2022 16:13:29 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbdb95dd3db1da9bfe68bf24ccb98e47681fc4cfa8ab474ce4efc25aff2ab07`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a65566fe525e381f5639a47cd2c97196e907894f6c10762ff3cae32fa1cdd3b`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863595908562193e85b1287222d90951da4cf1f7a075b4820e9da7b8d1b9a4da`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00292f0ba4bd525f47671337689f4d11e1ee966d077007a37eaae7fc0eda5bb`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d003cfef2605574ce4be63540f97caab8b329406d8c890067541e16081d8c4f6`  
		Last Modified: Wed, 26 Jan 2022 21:05:44 GMT  
		Size: 1.7 MB (1667078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21146e014bbacf566bd713a4d1a891e05e7f8da85f2cae49232335f811cb7f8`  
		Last Modified: Wed, 26 Jan 2022 21:05:41 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a6a37a033e28b11743049e8fc620b798a4e8fda291740c376b869184ff77954e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4886; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4886; amd64

```console
$ docker pull caddy@sha256:22cae5265f5cb60aa10f7a056b9281b4e61d0e14f16b5454f5b90f8c14e10e6f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6455446654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4079b70701d5a0ca0af10a7038d5f468c00e36871a95feb8e6e4926bda5e7d00`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 06 Jan 2022 14:33:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Jan 2022 19:14:55 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Jan 2022 23:34:03 GMT
ENV GIT_VERSION=2.23.0
# Tue, 11 Jan 2022 23:34:05 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 11 Jan 2022 23:34:06 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 11 Jan 2022 23:34:07 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 11 Jan 2022 23:35:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 11 Jan 2022 23:35:42 GMT
ENV GOPATH=C:\go
# Tue, 11 Jan 2022 23:36:45 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 11 Jan 2022 23:57:30 GMT
ENV GOLANG_VERSION=1.17.6
# Wed, 12 Jan 2022 00:01:53 GMT
RUN $url = 'https://dl.google.com/go/go1.17.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '5bf8f87aec7edfc08e6bc845f1c30dba6de32b863f89ae46553ff4bbcc1d4954'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Jan 2022 00:01:55 GMT
WORKDIR C:\go
# Wed, 12 Jan 2022 06:32:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:32:49 GMT
ENV XCADDY_VERSION=v0.2.0
# Wed, 12 Jan 2022 06:32:50 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 12 Jan 2022 06:32:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Jan 2022 06:33:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Jan 2022 06:33:58 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8428508ffd63b4af1ba690ec41e82a116f10ec6c3fb70962348f5448d42e5835`  
		Size: 2.2 GB (2208216859 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:9b5116c05ddf6ecb5a348f7628e3f3264afbb9909d86798316dbaff4a0e991a2`  
		Last Modified: Tue, 11 Jan 2022 19:35:13 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2caa59a1aaa1c092020bbca2ed4bb1396365f4d9d04ddbbd111ee689414c97a`  
		Last Modified: Wed, 12 Jan 2022 00:35:16 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9fe19533bf1afd7f80fd9cf407f00011eff59836d40dcceb1896e75ea99bf5`  
		Last Modified: Wed, 12 Jan 2022 00:35:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40700bafb918466fc1727b2e59ec5eb21d347affb09989cc72ac6db12220b882`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3180faaeb4219e7d41bb57faeebe12d142e8e246bac5ab81c8ef38499116de13`  
		Last Modified: Wed, 12 Jan 2022 00:35:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6189cfcbd5a7447e171b486da44213e8ff4721ecbf15998668c0b32e6fb06aaa`  
		Last Modified: Wed, 12 Jan 2022 00:35:18 GMT  
		Size: 25.4 MB (25440280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4766ed70813b67e83228fa314c288fe9a1998bb85cbbd29f2a4b0518e49a7c15`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8f2e04b601edd119e847cbb2468052ab4681cd44bf4e9bbdf9b6c3f792d0ae`  
		Last Modified: Wed, 12 Jan 2022 00:35:09 GMT  
		Size: 306.6 KB (306585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef103850c637e1ce1f8d175e0c4b5c7d6c2a3a29d2b8ad15bed8eab49be3dde0`  
		Last Modified: Wed, 12 Jan 2022 00:39:29 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce1f406ac407910a0724e1fbad6ed8772a277ce69316a98a2defcebb5320504`  
		Last Modified: Wed, 12 Jan 2022 00:40:03 GMT  
		Size: 149.8 MB (149846909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbdefe1352ad86026fe87510dd97f9a9acdbb5a700fc6a8aea2bd6eaa3194bd6`  
		Last Modified: Wed, 12 Jan 2022 00:39:28 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1578c0afb3c1729e44264a61a125be686ed8e738b033a03917b80f62aea0ed46`  
		Last Modified: Wed, 12 Jan 2022 06:35:55 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0d89ba8c66caec659fce7ea59e230983c2e8129e3026228cce6945904233cf`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e135d2e9e9a157d6d87f8f0e5e9cf6aef249cd9aac5e2b4313784e2d31664990`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715ab69f5d21664707eee604a40f003fbd665f65c14431d564a82a614b277496`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833db9ca0e9e1914a35515e476460cdd0bcc36174f85c13dd8646945c5199cde`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.6 MB (1631613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57f5273b431c8d65b59b81e63af176c5126e1b0d33f4d7b4ece422a1e01562`  
		Last Modified: Wed, 12 Jan 2022 06:35:53 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:af86498f48007129b4656236533520811fba83b2dd25e9e6f5ac5d59a4639f44
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:7da0f90273e1961d9c38d26809f84d4ef3cdc9b4fc330a9cab22015d7c9e8228
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14856906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439af64db48912c0a446444aae0e357183264ff08e1154fa105d5ee082e0bf13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 21:54:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 21:54:18 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 21:54:19 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 21:54:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 21:54:23 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 21:54:23 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 21:54:23 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 21:54:24 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 21:54:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 21:54:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 21:54:25 GMT
EXPOSE 80
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 443
# Fri, 12 Nov 2021 21:54:26 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 21:54:26 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 21:54:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ccae726125d77e2fd3891c69c8f663d5fe63d8ad4a67deb284e2c589334497`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 301.5 KB (301497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3de6a61c89acc2147364721befe6e6bf957963713d1ddc4bc6c4a35f7b4b4e0a`  
		Last Modified: Fri, 12 Nov 2021 21:54:48 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ed957bdc008c4cc475fcaeb053cdb7fbcc83f49184fca8013d87cf9d395518`  
		Last Modified: Fri, 12 Nov 2021 21:54:50 GMT  
		Size: 11.7 MB (11726445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ae44c2d42ddcf77445d391f491713e6384b933553eb234ceb0d9b3e66c5b33f`  
		Last Modified: Fri, 12 Nov 2021 21:54:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:caa4910dc3572e3ba3888fda3f7f5ed69c8c575461d29e528a6b453c0ba90522
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14068833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:358685e491b9f796f29e9b70a0a43f619fa034e7bcd995cf738d811cf8e4ebe9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 17:07:54 GMT
RUN apk add --no-cache ca-certificates mailcap
# Fri, 12 Nov 2021 17:07:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Fri, 12 Nov 2021 17:07:57 GMT
ENV CADDY_VERSION=v2.4.6
# Fri, 12 Nov 2021 17:08:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Fri, 12 Nov 2021 17:08:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Fri, 12 Nov 2021 17:08:04 GMT
ENV XDG_CONFIG_HOME=/config
# Fri, 12 Nov 2021 17:08:05 GMT
ENV XDG_DATA_HOME=/data
# Fri, 12 Nov 2021 17:08:05 GMT
VOLUME [/config]
# Fri, 12 Nov 2021 17:08:06 GMT
VOLUME [/data]
# Fri, 12 Nov 2021 17:08:06 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Fri, 12 Nov 2021 17:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Fri, 12 Nov 2021 17:08:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Fri, 12 Nov 2021 17:08:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Fri, 12 Nov 2021 17:08:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 80
# Fri, 12 Nov 2021 17:08:10 GMT
EXPOSE 443
# Fri, 12 Nov 2021 17:08:11 GMT
EXPOSE 2019
# Fri, 12 Nov 2021 17:08:11 GMT
WORKDIR /srv
# Fri, 12 Nov 2021 17:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d466a8f7766a93ea57a37532240c4a8c0e21cdb1f731360b1d21022b74f840f1`  
		Last Modified: Fri, 12 Nov 2021 17:09:28 GMT  
		Size: 301.7 KB (301671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:082eb2081a4e07ea8cd0a36b4c3e7fee48ac23e2f6e8b7f95659e9a7465012fb`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3790fd0e6afb978b6d8b451eaea5ab3e59b48913548a910853b31bc234bfed1c`  
		Last Modified: Fri, 12 Nov 2021 17:09:35 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe30a92d02271e636688f49fc9e1b382f2836b2c4578c29a993dc5111eb0b927`  
		Last Modified: Fri, 12 Nov 2021 17:09:27 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5211ef3cdd2abf233de36a5e914b3ea2a649f0ec2164e5c63dd96c0cf870004e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13852151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:389ecbea3a7d6a7b6a98da18b9b565046f2629b6c4af69a7d20d5cabcd1562d5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:43:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:43:44 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:43:44 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:43:49 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:43:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:43:51 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:43:52 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:43:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:43:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:43:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:43:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:43:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:43:58 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:43:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5663fa07ca1dcac265e40e084d2e40771a9084e9b30309c275bf810e87a3b53a`  
		Last Modified: Sat, 13 Nov 2021 11:45:26 GMT  
		Size: 300.8 KB (300831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8bc3ddae458c10861b1ef0a30a6c8e97ea3a7135680ced673a2532a4c043e`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afb06d1223418bbdf22f64f5a3a57962ad6570d931f931ab8df015439fb0c7a`  
		Last Modified: Sat, 13 Nov 2021 11:45:33 GMT  
		Size: 11.1 MB (11106718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a00e0b33a8465343d1f7f61ffec47a7c7aaad34402170530d9e9ebbb4ac5665`  
		Last Modified: Sat, 13 Nov 2021 11:45:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8c2b7f01f3d14048e888946dd85b972ac76d22490107d999f6df18399ab76f25
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13763680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e48a5247e105a4ecd7f6a7b3f6bfe21fe6633146de42ad9bd4197b3222b920d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:18:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 11:18:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 11:18:40 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 11:18:42 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 11:18:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 11:18:44 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 11:18:45 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 11:18:46 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 11:18:47 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 11:18:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 11:18:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 11:18:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 11:18:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 11:18:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 11:18:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 11:18:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 11:18:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 11:18:56 GMT
EXPOSE 80
# Sat, 13 Nov 2021 11:18:57 GMT
EXPOSE 443
# Sat, 13 Nov 2021 11:18:58 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 11:18:59 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 11:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e205c63fa7e1c7a1060c29f8600bf90d965a1d26a1ae313210de738d08649d0`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 301.4 KB (301450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674f75736ea40598c6df0d5460f914bf940c50952e8f106cdb674f9d98e8c5bb`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e004593c132f71a51cbd6967cf29bac3fc607c79fa8d967253c2f79461442641`  
		Last Modified: Sat, 13 Nov 2021 11:19:45 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51900aef2f22db52e1c14e6dd7f645241d02abef12b8ef2b377595f11b77055b`  
		Last Modified: Sat, 13 Nov 2021 11:19:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:b47a92735f1a101ce7087f2fc6f8b33614226b32c4507de0de8a4b6b34d84504
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13429323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49bbba192f1381ae73d2265be6a6b84d7539131fcc66399931bd66ff97ff83f5`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:14:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 15:14:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 15:14:33 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 15:14:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 15:14:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 15:14:54 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 15:14:58 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 15:15:03 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 15:15:05 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 15:15:09 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 15:15:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 15:15:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 15:15:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 15:15:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 15:15:26 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 15:15:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 15:15:32 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 15:15:35 GMT
EXPOSE 80
# Sat, 13 Nov 2021 15:15:37 GMT
EXPOSE 443
# Sat, 13 Nov 2021 15:15:40 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 15:15:42 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 15:15:46 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aca7d05e49e358a035d0dd6f471c0d19419c9cc97646fff4e82578d2c488237`  
		Last Modified: Sat, 13 Nov 2021 15:16:26 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc78b04675eccc541ab8678fe7221460039d23c40f04c02d41e150f256c4368`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f289e05d8a93edbe6667d481e3a61908205bf58c77aa2ddf18b09f740724a8cd`  
		Last Modified: Sat, 13 Nov 2021 15:16:28 GMT  
		Size: 10.3 MB (10302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd68deeff259e1bcfa76db665a6a52747267383f87bb506b77fbb409529ae3c8`  
		Last Modified: Sat, 13 Nov 2021 15:16:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:5ac69c24193df6b0d9b0c13816ce3861b720b62721901b0eb7446bd41ae86a3d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14240890 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:753d56e00623363d01fede6cee26039f1b7efc2f64fccec498168291c9b9ea6b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 04:01:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Sat, 13 Nov 2021 04:01:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Sat, 13 Nov 2021 04:01:38 GMT
ENV CADDY_VERSION=v2.4.6
# Sat, 13 Nov 2021 04:01:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Sat, 13 Nov 2021 04:01:42 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_CONFIG_HOME=/config
# Sat, 13 Nov 2021 04:01:42 GMT
ENV XDG_DATA_HOME=/data
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/config]
# Sat, 13 Nov 2021 04:01:42 GMT
VOLUME [/data]
# Sat, 13 Nov 2021 04:01:42 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Sat, 13 Nov 2021 04:01:43 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 80
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 443
# Sat, 13 Nov 2021 04:01:44 GMT
EXPOSE 2019
# Sat, 13 Nov 2021 04:01:44 GMT
WORKDIR /srv
# Sat, 13 Nov 2021 04:01:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0267ca443b43155e255c1a3bb35bab8ac5b561ddc2d0e768868f13274c7ab32d`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 301.9 KB (301922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b9c9c616a8868c7845a4a9d56e876f1bf42c37dac31b80761370b9af366e4c1`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c0dfff2c7fb2b8bde893d14f4d66fe6d6e8bee6115e0f4f691f7698d17a51f7`  
		Last Modified: Sat, 13 Nov 2021 04:02:29 GMT  
		Size: 11.3 MB (11323710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fc9ba4f178258a6de34c95f9f50fb0fd89e093f552c493cd511cfb5fc39a433`  
		Last Modified: Sat, 13 Nov 2021 04:02:28 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:70079683faad29699732179ae14ebd3ad2ef8330645ef775f581cf555496e15a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2458; amd64
	-	windows version 10.0.14393.4889; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:f504e734712cf31dc0903f54de87aa8791a825b7894d33a007da91b42a178a06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2458; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2458; amd64

```console
$ docker pull caddy@sha256:dbbf959ab8d12c9e1f64ecf1e64e839828e6a2210c62fc5dc777d49e6e7051d9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2726168484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d92470703f899a5df471154c8a61e8a98fa5fd6b17e2d627a9bedb8de3152316`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 18 Jan 2022 01:52:23 GMT
RUN Install update 1809-amd64
# Wed, 19 Jan 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 20:56:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 20:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 20:57:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 20:57:33 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 20:57:34 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 20:57:35 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 20:57:36 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 20:57:37 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 20:57:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 20:57:39 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 20:57:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 20:57:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 20:57:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 20:57:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 20:57:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 20:57:46 GMT
EXPOSE 80
# Wed, 26 Jan 2022 20:57:47 GMT
EXPOSE 443
# Wed, 26 Jan 2022 20:57:48 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 20:58:39 GMT
RUN caddy version
# Wed, 26 Jan 2022 20:58:40 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:567fd00846e9a9f44eea5925b497356dda00fe89b8335d2a3b2a8b9d84b0bb69`  
		Size: 995.0 MB (994988595 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba7b1090ce9545f6aac90d390785f6c5e3846304cb7596289dfc36c169d7b1da`  
		Last Modified: Thu, 20 Jan 2022 00:40:41 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40c2cef7b775df3a3981659855d54ad4b5d06fa31b80fac8935dc1d594c8e30`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 387.4 KB (387421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a405df0fcb30d9aed7e79492bf051fdf805cc2b61fc04402b0e19bb98099e`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ecaf8effba020fdaae6c4732000ac34efd20022528ce4f611f5b7d7240ed28`  
		Last Modified: Wed, 26 Jan 2022 21:05:00 GMT  
		Size: 12.1 MB (12134681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dabd3d287dd78fd75051d58c35912ce86d204ffb3cdeeb303b6f3889e74ec86`  
		Last Modified: Wed, 26 Jan 2022 21:04:46 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7810343cdb02640480b8f9e2ae59ea0bf2d10b0504240d6b89809ec1561a1db3`  
		Last Modified: Wed, 26 Jan 2022 21:04:45 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590277b2e5065c8a723c50774ff9fc1216dbf2154341f040e2c6fb960702ceb8`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657c093b0d6a43acec90f086209ec69b4cc72a5d81627542e897627a84ed330`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8df6f4cac7e903fa7d83dc00ab7413bb9d52e21cc4cad0e77edc8313285183b`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e21cc9c2d9450c09f274e267b4ab08d8156a14348bdb618eee3f1890fe6e2ba0`  
		Last Modified: Wed, 26 Jan 2022 21:04:44 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5300225bb76c81d44c64aef8c9e83411c7c8d527bb97b1cc5b7ff6e195394c90`  
		Last Modified: Wed, 26 Jan 2022 21:04:43 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a136ebe3e9b33bfec166c91e0d7981d7507f6d5e8033b148b7b43221e6eb6b4e`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26ebbf6d49755ae394c7f1bd27154075b74f728a3dbc40fdd919635cddd6341`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56892fed1c5488e43c67af4fc09dc12b497f59dd90158138b2ee27eb4e15e400`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9689920723864529f1beea5ae2e87729181895c58b58c3cd225f0dbe3dd8c9`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb710caf3adf67c3da420cc6cabb7a9b7524d60743519891e17ac6034316eb6`  
		Last Modified: Wed, 26 Jan 2022 21:04:41 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06f4f1945554888ddac36ff8ca137750672d829131157a9cc246c4ba31b11c`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98fe0704916e6888311e19571d0176a78bfd220f409970551c01c86e99007770`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d968c56fcc2a39d7c71cedded69a8e8c8da27ed7a6c3929f4b0a813eecc211af`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4575ff9c69502f35c8a7b0f31b0e7143aa6cb7a7b520c8ce636688f1fa969ba6`  
		Last Modified: Wed, 26 Jan 2022 21:04:39 GMT  
		Size: 301.0 KB (301014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e436fe120ba129e820476897cccec859c77a93e423bfc8470a3e984cc87f55d7`  
		Last Modified: Wed, 26 Jan 2022 21:04:38 GMT  
		Size: 1.3 KB (1301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:9f877e9983e295396f9d05504d82d70c7d34027e8fc2c3d86861ebec4932df59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4889; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4889; amd64

```console
$ docker pull caddy@sha256:eeeaaec1991ee88afa7d4642cda9c0bdbe77f7bdf9f27759e47452d13c419e0a
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6290311249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a77704a9a031c57790cc51ee74fec10fbbcded5138db006187f94a58e92a3499`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 16 Jan 2022 17:26:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 26 Jan 2022 20:58:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 26 Jan 2022 21:00:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 26 Jan 2022 21:00:19 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 26 Jan 2022 21:01:32 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 26 Jan 2022 21:01:34 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 26 Jan 2022 21:01:35 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 26 Jan 2022 21:01:36 GMT
VOLUME [c:/config]
# Wed, 26 Jan 2022 21:01:37 GMT
VOLUME [c:/data]
# Wed, 26 Jan 2022 21:01:38 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 26 Jan 2022 21:01:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 26 Jan 2022 21:01:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 26 Jan 2022 21:01:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 26 Jan 2022 21:01:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 26 Jan 2022 21:01:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 26 Jan 2022 21:01:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 26 Jan 2022 21:01:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 26 Jan 2022 21:01:48 GMT
EXPOSE 80
# Wed, 26 Jan 2022 21:01:49 GMT
EXPOSE 443
# Wed, 26 Jan 2022 21:01:50 GMT
EXPOSE 2019
# Wed, 26 Jan 2022 21:02:33 GMT
RUN caddy version
# Wed, 26 Jan 2022 21:02:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:632aaeb77a49daa93237d42e634f5d4574b96f1dafbdbe1e066e9d1341211c49`  
		Size: 2.2 GB (2207519242 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb80ff8c3e5af742d68a82ac4184bf4bcd4c4efac0ec02c4cdca44e2a58a0c1a`  
		Last Modified: Wed, 26 Jan 2022 21:05:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c21feeed0335fc6c5a873eaa9c855febb47d816e00c480321a1bd71582818c3c`  
		Last Modified: Wed, 26 Jan 2022 21:05:23 GMT  
		Size: 345.1 KB (345102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c861f81a6c7ab1b39e184f410ca0cda8f77d625b8c05105368eabe90badd290`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e272a931194ddbbc869d38fdf0861be05329b07df5bae359c5a2584dd34bc03f`  
		Last Modified: Wed, 26 Jan 2022 21:05:26 GMT  
		Size: 12.1 MB (12139707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95449a73e0fb2b4556362289cb59431cc7d3f366b4c8527ea2beeb1682633b`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4224f5ff81fd270cfab3ca30c450c1802fb53da437a5ef6d08b200557222c9`  
		Last Modified: Wed, 26 Jan 2022 21:05:22 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50c1bff263ca980844d0d2496ce9c34db3cf665fe7315ba5ac7fde2cb676d52`  
		Last Modified: Wed, 26 Jan 2022 21:05:21 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dac40fedacc0645b496cc66210bbe98b94e03851c9ae4f6ba65518fa904a6ac`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f84d03efadea644d38785a84dc1a2ea5a1d202ae0977ea9099904495a4f235e6`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f19b5dd8318386399626a1d053855e69c5c2b03e076cefa91753e848e11f26e`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba1f05955408fecb76702f1fabc75a51062083c789224e91b185b2fb4b50390`  
		Last Modified: Wed, 26 Jan 2022 21:05:20 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1882b675e313427e12ef4aa044b93d35e56e1fda6217b0f7879ab81701c6dac1`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca7c70fbf9e825b2ca46a9ffa3af8d33011e35a8309addc9688331b81a78728`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2b143ffdcb9ac54b198752f80ee39bd584936ff41093af21beed9ab0335f05`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a1d61050af904a8fa73b00d2835bc8d925d1a9d1fc7bb2cebc8e2aa25caae3`  
		Last Modified: Wed, 26 Jan 2022 21:05:17 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e371c54b20f4e20315f67b665e8c69dc580155bef88300ff246093694fea22a`  
		Last Modified: Wed, 26 Jan 2022 21:05:18 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ca59663a81ec07f51de6478e6f7490bebf90b57195167390d391dfbcfa45fb`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f99d5a9796d1dfd0581d82cadac1923fa05095f69e93a35c330126873adee27`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dfb267ffa78d4814f31be21f9dfd3ddc19a97739a9d1453b43e290d0b0f6878`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904f511a0ba6304c1dfe785f40b4976669f23c45b0a772b1a09c2121947e38a8`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 297.3 KB (297325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df98ba8017f31cf68d84c1a4fe2b4829db49d744e91831ba8749d3d9fbca9f42`  
		Last Modified: Wed, 26 Jan 2022 21:05:15 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
