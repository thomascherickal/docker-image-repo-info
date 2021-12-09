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
$ docker pull caddy@sha256:46f11f4601ecb4c5a37d6014ad51f5cbfeb92b70f5c9ec6c2ac39c4c1a325588
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

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

### `caddy:2` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
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
$ docker pull caddy@sha256:05f450e87273719b9a63d2b96bc8dd7f1c51ed7e8d5edd44f7de26e5731e15d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:a305dcec87142bca20205a4010687c5e2515ad0b98de23cf74953110d477d855
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
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:100d6c1c7a3bfa2fee20e6febfdd9aaa44924ff26e0881f5a720c86d5ee5786b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b062317bd31936b3f57d25dc554159fdab9f6a60fdc41d81ca410fbe72bc6da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:3864aebe0cb9d8ec8b0707762c6637cf9ad27a88bde3be6f9d0842eb01a19666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4d8f28e3fbdc28a6ebdf57a867626560f0651157d3cf1cddaa279a9f57c34c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b399e4134eac2ed1e68a9f6d12fa6c2f89351edd4b13f45e687d84ee2c8c7891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6`

```console
$ docker pull caddy@sha256:46f11f4601ecb4c5a37d6014ad51f5cbfeb92b70f5c9ec6c2ac39c4c1a325588
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

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

### `caddy:2.4.6` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
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
$ docker pull caddy@sha256:05f450e87273719b9a63d2b96bc8dd7f1c51ed7e8d5edd44f7de26e5731e15d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:2.4.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-alpine`

```console
$ docker pull caddy@sha256:a305dcec87142bca20205a4010687c5e2515ad0b98de23cf74953110d477d855
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
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:100d6c1c7a3bfa2fee20e6febfdd9aaa44924ff26e0881f5a720c86d5ee5786b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:2.4.6-builder-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b062317bd31936b3f57d25dc554159fdab9f6a60fdc41d81ca410fbe72bc6da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:2.4.6-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore`

```console
$ docker pull caddy@sha256:3864aebe0cb9d8ec8b0707762c6637cf9ad27a88bde3be6f9d0842eb01a19666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:2.4.6-windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4d8f28e3fbdc28a6ebdf57a867626560f0651157d3cf1cddaa279a9f57c34c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:2.4.6-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b399e4134eac2ed1e68a9f6d12fa6c2f89351edd4b13f45e687d84ee2c8c7891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:2.4.6-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
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
$ docker pull caddy@sha256:05f450e87273719b9a63d2b96bc8dd7f1c51ed7e8d5edd44f7de26e5731e15d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:a305dcec87142bca20205a4010687c5e2515ad0b98de23cf74953110d477d855
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
$ docker pull caddy@sha256:c6c8aae1fc1dfdc75df0d570601d559e23f236e8be0b4ed0f7953e37a7f34587
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121296055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1f3ecc274acf640ff5f6c719fc15ae2b3546128a8daced1589aa2b08bf31459`
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
# Thu, 09 Dec 2021 16:21:02 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:23:11 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:23:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:23:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:23:13 GMT
WORKDIR /go
# Thu, 09 Dec 2021 16:52:07 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 16:52:07 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 16:52:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 16:52:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 16:52:10 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 16:52:10 GMT
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
	-	`sha256:1ff5b6d8b8c6b6093e19083f398755431fee6120fae681379ad828e84f387ec0`  
		Last Modified: Thu, 09 Dec 2021 16:33:27 GMT  
		Size: 110.1 MB (110128496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40fcfd711f8db74e87407ed47c1d306a77eefe885d79679595d94f13c905f395`  
		Last Modified: Thu, 09 Dec 2021 16:33:13 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598ab90f7304c0b00d688604144334d3062f737f6daf8bd0fa12e9c99d4537b4`  
		Last Modified: Thu, 09 Dec 2021 16:52:31 GMT  
		Size: 6.8 MB (6821302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf6a9d71af7233285ce3c5e0438c30d3fc2946e7ab70148b69b719a8e38ee77`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 1.2 MB (1244970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe6e8da726d62502bbd028afc3c8b548f96c466b4b282f555d7443691b41b5d`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c535540cc2417a2ef41d94e8acc90532407bcbb17f4c546fa966254b1fad8d6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115762499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe12c8038fdaaaf41989486892530c351ade53032b3a6df42dc1a5d073966632`
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
# Thu, 09 Dec 2021 16:49:38 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:53:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:53:08 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:53:09 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:53:11 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:53:11 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:26:35 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:26:35 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:26:36 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:26:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:26:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:26:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:26:40 GMT
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
	-	`sha256:8c6102918e3ce0854a1fbb1c3058dcba811e709a8aca743460799cc6585cdce8`  
		Last Modified: Thu, 09 Dec 2021 17:05:46 GMT  
		Size: 105.0 MB (104993607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab16c6a73210154f0f547f5e5c92164761dbedf793297e3ec93944e8941a0a89`  
		Last Modified: Thu, 09 Dec 2021 17:04:37 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfcb0e06645de846388a91f52116fcb970cf75b7c835de146d02242d535b7d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:47 GMT  
		Size: 6.7 MB (6677084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c6932b6a995dca9062ba7094180af8cc1673b7909b1e265ad8e1afe3fc0492`  
		Last Modified: Thu, 09 Dec 2021 17:27:44 GMT  
		Size: 1.2 MB (1177565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64ac8ea1aa213a08d5a867e055bf9265a9723562a784df90f965bcf74e3256d6`  
		Last Modified: Thu, 09 Dec 2021 17:27:43 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:5f6554f2b0754381592d1d07197643396cfde71caa8e8ad8ee0c1a4ca69b1161
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.6 MB (114630160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11b7247d8504f7c586fb9af0d32c69ed0a46600c4f41b0c87c956c9deae3846a`
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
# Thu, 09 Dec 2021 17:00:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 17:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 17:04:17 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 17:04:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 17:04:19 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 17:04:20 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:49:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:49:30 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:49:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:49:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:49:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:49:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:49:35 GMT
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
	-	`sha256:974ed2bee41b58f27040b2b46239bea5cb18484cba960ab9233c113c0ab228a6`  
		Last Modified: Thu, 09 Dec 2021 17:24:54 GMT  
		Size: 104.8 MB (104785572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa26dd433ddcc5c41b58ce01b8e3df28cbde0028536598633dba4f4b4b19319`  
		Last Modified: Thu, 09 Dec 2021 17:23:46 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8bfe65c7114d3c6872aeac5a89543947861b666163bb1eb88753be650c27be`  
		Last Modified: Thu, 09 Dec 2021 17:50:42 GMT  
		Size: 6.0 MB (5951594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9414a599c395ed545b225372db794545a92110cfdbe8472bd360fd57937060d`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 1.2 MB (1176266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f02300db4ae4637c3e61d5f3d7c8b430a70a6de204b596b509aedc441250eca3`  
		Last Modified: Thu, 09 Dec 2021 17:50:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b69558abae21e3fd9c277b903d130d46c840e5940db73970192996d348e867d2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115441646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98781c03c659307affc1942c4803e4331144f3914ad856ddc99bbca736187139`
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
# Thu, 09 Dec 2021 16:41:12 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:42:40 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:42:41 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:42:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:42:43 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:56 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:57 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:11:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:11:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:11:02 GMT
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
	-	`sha256:52f1d2cc2047096fccb9e9c98a434c2b4673cde748c1a935baaef4e1a3113c49`  
		Last Modified: Thu, 09 Dec 2021 16:52:03 GMT  
		Size: 104.4 MB (104369707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79ebd5bc6f15dff169efe2a6f424f776b67bdef8c956da543bd768ca7262f85`  
		Last Modified: Thu, 09 Dec 2021 16:51:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0ee2f33ae1743b579ca8cc13c6c2de8e5e84b67cad0789db7620d8e5d9d841`  
		Last Modified: Thu, 09 Dec 2021 17:11:34 GMT  
		Size: 6.9 MB (6925798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d20fe1d9d9904836b4c91d38b8157f4586ce579a5239b89c3d98e3674b60cad`  
		Last Modified: Thu, 09 Dec 2021 17:11:33 GMT  
		Size: 1.1 MB (1148123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4b2783718d896894ab43a03c922a5dca79c6e9b923df57558e7b8d1c77c3db`  
		Last Modified: Thu, 09 Dec 2021 17:11:32 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:75fe3460029e2f8cb4d3576d086e12040b0b7021fc67ca4d6bf7c159be78b95f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114267571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:008e9825f8ba43a187d57b2a45e4b2ebeb69238b5be3a2c374a377672b43e71e`
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
# Thu, 09 Dec 2021 16:18:52 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:21:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:21:16 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:21:17 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:21:23 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:21:25 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:30:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:30:36 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:30:42 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:30:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:30:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:30:58 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:31:00 GMT
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
	-	`sha256:112fa878e5c02b4c5dc0be6726e6cca9dffaadb4ce2a103a6dbf294a31817260`  
		Last Modified: Thu, 09 Dec 2021 16:36:11 GMT  
		Size: 102.7 MB (102727609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a27ba9fb84b49ca3b6930f8ea26568eb6a8225917e42a928844e570a24bff46`  
		Last Modified: Thu, 09 Dec 2021 16:34:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8154f22c05183c07c7e255a2bfe325c562a69c76074fe571e740af1a239bec55`  
		Last Modified: Thu, 09 Dec 2021 17:31:36 GMT  
		Size: 7.3 MB (7320433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5556d31c6a0c454106f29c2ef178d8ae6be73f3ce9eecfd5a8f05b2e687d6e3`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 1.1 MB (1120014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545ec282a6a0dc6e5300516dad0169450cf79017c158abf7da499fb24aba847c`  
		Last Modified: Thu, 09 Dec 2021 17:31:35 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:7106c5ea2ca27bf730919cb1efee3ca8302b4dc39603983845216e2d446f00c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118687949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f952b76a7f32bd7c3999ec87d9a4ffbc7776e1214b0dbef2929601efd224742e`
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
# Thu, 09 Dec 2021 16:42:55 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:44:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.5.src.tar.gz'; 		sha256='3defb9a09bed042403195e872dcbc8c6fae1485963332279668ec52e80a95a2d'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				go install std; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 09 Dec 2021 16:44:32 GMT
ENV GOPATH=/go
# Thu, 09 Dec 2021 16:44:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 09 Dec 2021 16:44:32 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 09 Dec 2021 16:44:33 GMT
WORKDIR /go
# Thu, 09 Dec 2021 17:10:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:10:14 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:10:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:10:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b02fef09e1ea4ec26d87f1d24a442aaf247ca79b391064d7708e080e4bc5e14204381a3c573122b8b5f10de4495cf4e54fd7b90122ed45127673284d9619a0b8' ;; 		armhf)   binArch='armv6'; checksum='735f5327e47d7a4fbc224b305231f211475b26f7a0def11eccabc15c98fc1864f36370de235869a093a3c97a7ebe1ca255a4e64ab4eaf77dae89bd8a28a708a0' ;; 		armv7)   binArch='armv7'; checksum='d013d38f62ca548dcdea532224cd8571975d2b8c9bfcf98fc392907fd97d0ecfd0516d457b32988ef7215c626d51df2c2b6ca17f7c3cc14db656b84d4b1b8304' ;; 		aarch64) binArch='arm64'; checksum='d64fbed9556bf3997951d5337b91eb85b2a3abf3bf6d3e28a838f1977c276e39087e435b6def9a860cdd6d1f0095602374ddedb3e6c382b8a29c7d446623f651' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b304e6129e4928155c1c9eda33b76b43024ba34bd0197445a8dff12b45472f92d96d90b9083525b480d796d94bfe861cc415b4dbaad56cfcc5e6f1c366cc476c' ;; 		s390x)   binArch='s390x'; checksum='ad3b5e27804d77f76429c98babf8df6f3418b613ec94370afc57dab5ed7f9b6492118f6706b01d73f1ff352c3f5618f41cb87dfbc3b089b2230d064bd8153a41' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 09 Dec 2021 17:10:15 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 09 Dec 2021 17:10:15 GMT
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
	-	`sha256:96da0cdd873834ffa52e45c34d792f710b7ea7116482dea0db978d844d9d7c92`  
		Last Modified: Thu, 09 Dec 2021 16:52:30 GMT  
		Size: 107.7 MB (107664790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3dd5717bef2c63c87ea66fe241d1f34d97265a9e03e0b9cbac24068b097b8`  
		Last Modified: Thu, 09 Dec 2021 16:52:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:432f13b7a5cbc9377fdd30c8283d56466107b2a074cc1d54584570baeb036560`  
		Last Modified: Thu, 09 Dec 2021 17:10:52 GMT  
		Size: 6.9 MB (6930615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a3a3a16415f2d37987270c8eeab91217bb34f6c6fe68ab0fec97d29420f91b`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 1.2 MB (1203508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4b783e107beb007bead2f1c8267f69b4484cdbd9f1ffacc682b0b91ad84d4ad`  
		Last Modified: Thu, 09 Dec 2021 17:10:50 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:100d6c1c7a3bfa2fee20e6febfdd9aaa44924ff26e0881f5a720c86d5ee5786b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:ab77c9f5d1117d4e18e15a095e01bf618ade99e0b662e8456a4c77dd30c61d3c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2879052852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a8300ff974c49903c4ccbfb1f717befb4223f965c5d12da34250c24200c1857`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:26:17 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:26:18 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:26:19 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:26:20 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:27:37 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:27:38 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:28:31 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:18:06 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:22:20 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:22:21 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:22:36 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:22:37 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:22:38 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:22:39 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:23:55 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:23:57 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f32622fe466bd678a47b75fa13ebb7781336e6a776a22f424036aa8e91fe1d`  
		Last Modified: Wed, 10 Nov 2021 14:05:07 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d684ea4a6b52df2d3b5c7f7876e3b784ff1def8eb60f9637d920f4e0e7870b`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ff61f0f89258dd1f49b766ef30baddd8f3e3821737778748ba95b52c1a480c`  
		Last Modified: Wed, 10 Nov 2021 14:05:03 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e16dc9a497b44a664b28524686ca0e75c6a244af505429f54f80a6aaa96c7af9`  
		Last Modified: Wed, 10 Nov 2021 14:05:04 GMT  
		Size: 1.4 KB (1448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e724f5e2b6e2fb2598ad100e7efa9cf30fe013f56537a5587d8e8868ae82d50`  
		Last Modified: Wed, 10 Nov 2021 14:05:09 GMT  
		Size: 25.4 MB (25446198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84e37bf01f689e54241d5e76695c5cbcc3313f3f8a85748e9d086c6cf3e4c3d`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f6ed9286b06435dae34f3d3e03f2c62a4415e3703740a83381b4ac0a3d1804`  
		Last Modified: Wed, 10 Nov 2021 14:05:00 GMT  
		Size: 325.4 KB (325448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5aaa5285e3d69dd098ab5c0f1caa98965bed4c9857770d57355eaf405d8234`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7720193a71ef0e3817b2ac002ab4390f1ee284cf12060b5ba0771a9abea7437f`  
		Last Modified: Thu, 09 Dec 2021 16:53:50 GMT  
		Size: 145.5 MB (145462133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b85cafdd9526732bb93ea6a7dc6ca348c4d82163963ff6a4303dd95424fe2`  
		Last Modified: Thu, 09 Dec 2021 16:53:15 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034258b8eff358d2b07cbb2c3adcfde0262ac7e401146280af34dafe47a0bc4f`  
		Last Modified: Thu, 09 Dec 2021 17:26:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64f6a8716364181bc80858519a9ec9a34e9d77d089b7263e6f8fd1d20514a91`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94208548e1d9f26cd3eb1ada046796ce9ed3f07ce1bc48d3795c53991db1e56c`  
		Last Modified: Thu, 09 Dec 2021 17:26:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e897dacf9234a67859767ee305da94400052a8ee97c8ed7b806c988196eb41`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75805724ee8b10eccc073013d071dcff7082022c0269289753d0e160c28fd26d`  
		Last Modified: Thu, 09 Dec 2021 17:26:16 GMT  
		Size: 1.7 MB (1679308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:482e0e23d20de7f105e84031f9780e121f06255c6fbe5e8893ff8e3aadb7edfe`  
		Last Modified: Thu, 09 Dec 2021 17:26:14 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b062317bd31936b3f57d25dc554159fdab9f6a60fdc41d81ca410fbe72bc6da0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:d1c1ea0b97aa180ac5d9dd6d4b87e6c8751f90a6843a332c50b24b3e26074993
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 GB (6450525247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce23c5cb4b80bb9007fd3f07fda02a57dc10732aeb51b6a08ff19a0873c10a8d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 13:31:46 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Nov 2021 13:31:47 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Nov 2021 13:31:48 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Nov 2021 13:31:49 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Nov 2021 13:33:35 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 13:33:37 GMT
ENV GOPATH=C:\go
# Wed, 10 Nov 2021 13:34:34 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 09 Dec 2021 16:22:39 GMT
ENV GOLANG_VERSION=1.17.5
# Thu, 09 Dec 2021 16:26:50 GMT
RUN $url = 'https://dl.google.com/go/go1.17.5.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '671faf99cd5d81cd7e40936c0a94363c64d654faa0148d2af4bbc262555620b9'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 09 Dec 2021 16:26:52 GMT
WORKDIR C:\go
# Thu, 09 Dec 2021 17:24:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 09 Dec 2021 17:24:04 GMT
ENV XCADDY_VERSION=v0.2.0
# Thu, 09 Dec 2021 17:24:05 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 09 Dec 2021 17:24:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 09 Dec 2021 17:25:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.0/xcaddy_0.2.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('233a57384b1f82e9420567da74b4fbd19e898112e43b8447dbdb8ddde15cb4d8a66aea58307ccdda74d37c5e525f0dc563f83d4670aee048842754eee9a3bc2b')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 09 Dec 2021 17:25:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a0c69f83a30944f5afdc948b3583f1418f71f3ae5a02382610f0898eb501f9`  
		Last Modified: Wed, 10 Nov 2021 14:05:54 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29e4bea9e4e2ccac41591b4aed9981453c554ca498a23d01a69638d6ccab7016`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b36358e1913c99dc66fbbca2e4c0f8472796bf33ceeb7fdc02d2b7096b1208d`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d071f5d45753629193f76196d769df9ff71ce3a39e5b10a16ff571cdb071a902`  
		Last Modified: Wed, 10 Nov 2021 14:05:52 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e79602be6489be8a0e5e82221cae33eae5692897081a79bfe959604121e2d0a4`  
		Last Modified: Wed, 10 Nov 2021 14:06:20 GMT  
		Size: 25.4 MB (25448073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f30d749fb8ba78fba5cce783b8cbe233632a2ba5965d4b67168111396620aaa0`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f08b5963e19f3d28aa336d06434d4efec179b4b813e4aa4222ab064bc180f7`  
		Last Modified: Wed, 10 Nov 2021 14:05:50 GMT  
		Size: 354.9 KB (354902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957f23f505ada08be66da657b8c5d20ad584bf8c5cd4f8210e4c2de3dff14397`  
		Last Modified: Thu, 09 Dec 2021 16:54:07 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ed41a78732c54eb7349ee63c6b6d8120eb22db3cad512d05e6a1e52803d1b73`  
		Last Modified: Thu, 09 Dec 2021 16:54:43 GMT  
		Size: 150.0 MB (149957582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d2a712bf1586c5607c4a51240ca803c310512a3e0d5f9fff182afe25e9b33f8`  
		Last Modified: Thu, 09 Dec 2021 16:54:06 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8e373b4b1373162321af7ffd49da4854d59d823b1bd4eb11bf14a4ce23563b`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2e39aab83a036f143f327df0eeca78d30e2fe4542bca5d3b69d10f28eb7005`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c635e14e9c42f3bd9f47c0702d702f4b9a74b90e2e138124c6de9eb9c8ee19da`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d210372bfa8e1614a6089e42da5c51314c8d7dd954aeb596063a4022c4b35f79`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56cb318149336e12e9481da8167ed6d17d98c1e7350aa4a86164af73be951066`  
		Last Modified: Thu, 09 Dec 2021 17:26:33 GMT  
		Size: 1.7 MB (1655375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71061f032e84a1fe6882c4977230537d06eac067f9a5f63fef64eb99d40b6ec6`  
		Last Modified: Thu, 09 Dec 2021 17:26:30 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:46f11f4601ecb4c5a37d6014ad51f5cbfeb92b70f5c9ec6c2ac39c4c1a325588
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

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

### `caddy:latest` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:3864aebe0cb9d8ec8b0707762c6637cf9ad27a88bde3be6f9d0842eb01a19666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:4d8f28e3fbdc28a6ebdf57a867626560f0651157d3cf1cddaa279a9f57c34c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2300; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2300; amd64

```console
$ docker pull caddy@sha256:4a8d9dccf760a0249237dfcf9726c0eb1b06e0b19f5ff67cf8718f8da29507c5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2718934999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ea4590fabf41404b64c9e90299fd322ac88350fd817d631f26264b5915ed362`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 01:42:03 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:12:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:12:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:13:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:13:19 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:13:20 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:13:21 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:13:22 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:13:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:13:24 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:13:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:13:27 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:13:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:13:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:13:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:13:31 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:13:32 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:13:33 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:14:19 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:14:20 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b35c0957cca5902f3108e43a3c2c11250dc754ee0bb43900eb0719b4350f0bc2`  
		Last Modified: Wed, 10 Nov 2021 02:08:44 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4b6e8b6a9caee6f47bdb32f6ec53fd2836fc02cddea3324c72caf380622fc31`  
		Last Modified: Wed, 10 Nov 2021 20:20:37 GMT  
		Size: 370.6 KB (370576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0308f92ecf7a222e22b826cf5c198551ffc380b76ee3e8de67da904b4b02f873`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df7693285564a1ff855781db06d1dab2fa702b5492fd55461fc675cefb47b6`  
		Last Modified: Wed, 10 Nov 2021 20:20:50 GMT  
		Size: 12.1 MB (12127869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a1d26d8d7789115491377813de4a8a0c15aa4772e3b22b229a4a061f4994d5`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766e31d6b0534ea731f651ccd59e3397360e7878802aaf90257635b0edd37086`  
		Last Modified: Wed, 10 Nov 2021 20:20:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b6f52680a8e584e06bb957343f7acef41f8863af076fed0c94c583f6a6a8ea`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3be75f11ed2b624d7b0d85454d91e6ba425c4b11d179b44611f0353c75976a5`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31bb0fed8a1d238828c7b967ddc9453e83dc38e811f50de90a87ca4a79677e3e`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3343adb9cf1bed7b331007eea1fb0bfdcdcc2a11c2c295d513a73d451d338298`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655ad263ab440756e44a5b758408a577f4ba4e960ae9daec72945afc3047553f`  
		Last Modified: Wed, 10 Nov 2021 20:20:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d09b8e61a4bbdc190857116fd8fc09cd71a5409e0bf984c7a033272b2ef5f5bb`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9723996732fa25ff5ef95b4bd85c9ddf6dfd27408fe9e220bf0156031ade487d`  
		Last Modified: Wed, 10 Nov 2021 20:20:32 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d58c78cd1d1a8562bd34f68b10ada8622f98bf19ad87174e2a3810657e48e70`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67885c8112bf51b21d408141b4bf3b2e13f08f96cdcd873dc6ca1310bdf08f65`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77274081e32b6ce8f84a136cb45008f07cd542a8f2fa0cb8a355331280e27248`  
		Last Modified: Wed, 10 Nov 2021 20:20:31 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acafd6faed9e989da5b7ca4bcf5d704b15d86d0b5076b645224a578b5453eb61`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:109d2337e42e4f8cfc28c01475b5d1ab49d1e776006c622915ec2166c8fead72`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ee8d0bd71b0b4f05c46aa89f1434f50b4685f23ab7e0e092ae5f46e1d150ad`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd8ebab410bbbe5d576ac2f9ec8f4f2b9d251ae4a307bc8c11bb47165553f63`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 290.2 KB (290194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a550a1217bcfc790088e7a6d4f32ebdea15bae25f297c4683cb3dfc3e6c72e4d`  
		Last Modified: Wed, 10 Nov 2021 20:20:29 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:b399e4134eac2ed1e68a9f6d12fa6c2f89351edd4b13f45e687d84ee2c8c7891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4770; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4770; amd64

```console
$ docker pull caddy@sha256:2c091f3638b3d3948ffa8c2d95a9be662e858768ffc52e366872371a68d003a1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6285957464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12fb2d13bfaf3ee5703b28aa6d939cbfac5b14658e1e3e91bbae594e1c4b22a2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 01:53:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Nov 2021 20:15:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Nov 2021 20:15:35 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 10 Nov 2021 20:16:38 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Nov 2021 20:16:39 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Nov 2021 20:16:40 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Nov 2021 20:16:41 GMT
VOLUME [c:/config]
# Wed, 10 Nov 2021 20:16:42 GMT
VOLUME [c:/data]
# Wed, 10 Nov 2021 20:16:43 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 10 Nov 2021 20:16:44 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Nov 2021 20:16:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Nov 2021 20:16:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Nov 2021 20:16:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Nov 2021 20:16:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Nov 2021 20:16:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Nov 2021 20:16:50 GMT
EXPOSE 80
# Wed, 10 Nov 2021 20:16:51 GMT
EXPOSE 443
# Wed, 10 Nov 2021 20:16:52 GMT
EXPOSE 2019
# Wed, 10 Nov 2021 20:17:30 GMT
RUN caddy version
# Wed, 10 Nov 2021 20:17:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:68d5dfbca608972a02b334e8d053010ece888346d5ebabfc28c9f91ed2063b15`  
		Last Modified: Wed, 10 Nov 2021 02:10:39 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:224cfcc2d1317d73465188f71867febbba9a64bbfcdf83b35bccd662bdb25748`  
		Last Modified: Wed, 10 Nov 2021 20:21:11 GMT  
		Size: 366.8 KB (366836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98f673e7fe75a29f4060341dab79e20ad059162395f10fb1fc2504379d12f22`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dc3d9f8e8e85985894d372a912cae2cbc64cc10540262498597bbe8cad8c31`  
		Last Modified: Wed, 10 Nov 2021 20:21:24 GMT  
		Size: 12.2 MB (12158174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197a3f340985e5e76e3ae77fcbb9e208f521abbad0cfb8921d27d4afe569f280`  
		Last Modified: Wed, 10 Nov 2021 20:21:13 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1443a981044b58af1bae85624fffe4dde7c1759e6a5f930ddaf2eb70bc3185dd`  
		Last Modified: Wed, 10 Nov 2021 20:21:10 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1b023614dd84860e7a4fdd1855131b5478b9b747a40fc9383467934e48e310`  
		Last Modified: Wed, 10 Nov 2021 20:21:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daca4ab6367b318ae3a2df27bbe0c53c12ee1a0196fc4f43a43ec47acd74c7c`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a288866cea4075f0f825973ce9d3369dd9411f73c325ed870a5233b383476dbc`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ea1c63b1b4cb8f39b59025d926f384679d17bb660eceafe7f7c9418dcdfad61`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b25f60f98964a2d03947e1dac0b01388ad6c9c65497e546f8efe7f2fdcd35e`  
		Last Modified: Wed, 10 Nov 2021 20:21:08 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d10f21fe32d5dd37a74db003c1119b2aaba639690b10ad4c46d22e2699140fc`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4bd5845100c889806835753480fb0016610fbfab35d197c6aa641d73c114ed`  
		Last Modified: Wed, 10 Nov 2021 20:21:06 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190767770423c20b77f963553559cfa26d18b490228ad11c4f9fcf62e6dcefd7`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab0412df33f87a4e77ce1ef8afc68a04cd9a9a56ce9a21e3494f4e4f7c1083a`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a80edcc113a751c789aee343b18fdb12c9099cd642cf099ab6a962c7cb0bce8b`  
		Last Modified: Wed, 10 Nov 2021 20:21:05 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d513b74afabeb0e8050ca955cdf8b72040cabc21350ab394862808bd4382649`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc99c5e78f676bc2fed853c2d43f71dedcbf29fe3a6f69f5d0bc1eabca7f8e98`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1532dfe2f3d7f9a4d2eed5ac842a7b54e160fb4d856388e1153d0c6488bab749`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c6594f3623b09c0359fe4347b1981678cebb55cebad4bd683d4bc059e0a201`  
		Last Modified: Wed, 10 Nov 2021 20:21:04 GMT  
		Size: 316.3 KB (316295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c07c5e836014edc4e052889ecbe945aa470b434f2563726bd4f9684da37bfc1`  
		Last Modified: Wed, 10 Nov 2021 20:21:03 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
