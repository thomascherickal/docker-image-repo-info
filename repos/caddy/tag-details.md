<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2.4.6`](#caddy246)
-	[`caddy:2.4.6-alpine`](#caddy246-alpine)
-	[`caddy:2.4.6-builder`](#caddy246-builder)
-	[`caddy:2.4.6-builder-alpine`](#caddy246-builder-alpine)
-	[`caddy:2.4.6-builder-windowsservercore-1809`](#caddy246-builder-windowsservercore-1809)
-	[`caddy:2.4.6-windowsservercore`](#caddy246-windowsservercore)
-	[`caddy:2.4.6-windowsservercore-1809`](#caddy246-windowsservercore-1809)
-	[`caddy:2.5.0-beta.1`](#caddy250-beta1)
-	[`caddy:2.5.0-beta.1-alpine`](#caddy250-beta1-alpine)
-	[`caddy:2.5.0-beta.1-builder`](#caddy250-beta1-builder)
-	[`caddy:2.5.0-beta.1-builder-alpine`](#caddy250-beta1-builder-alpine)
-	[`caddy:2.5.0-beta.1-builder-windowsservercore-1809`](#caddy250-beta1-builder-windowsservercore-1809)
-	[`caddy:2.5.0-beta.1-builder-windowsservercore-ltsc2022`](#caddy250-beta1-builder-windowsservercore-ltsc2022)
-	[`caddy:2.5.0-beta.1-windowsservercore`](#caddy250-beta1-windowsservercore)
-	[`caddy:2.5.0-beta.1-windowsservercore-1809`](#caddy250-beta1-windowsservercore-1809)
-	[`caddy:2.5.0-beta.1-windowsservercore-ltsc2022`](#caddy250-beta1-windowsservercore-ltsc2022)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)

## `caddy:2`

```console
$ docker pull caddy@sha256:f4840526af7bf068e5e8941e190bb42c0c8e98f10b2ee576d92ff85cba9d368d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:dd418a7216b6f833804da6b82fb215b7659f22ba7dd0196e201b2266dc2fd095
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
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:0a75456de360e6bdb884196a71cbbc5cedc0ec95b9cbd5c86a0861f8e3115c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:47fbe5354ee0e56faaab47d85cd0e212914290367b7815eaea9175387a081145
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
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:276530503290de9ae8be7471e975d5db1e0d286e99d48317b675cec03c7c2fca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6`

```console
$ docker pull caddy@sha256:f4840526af7bf068e5e8941e190bb42c0c8e98f10b2ee576d92ff85cba9d368d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.4.6` - linux; amd64

```console
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-alpine`

```console
$ docker pull caddy@sha256:dd418a7216b6f833804da6b82fb215b7659f22ba7dd0196e201b2266dc2fd095
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
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder`

```console
$ docker pull caddy@sha256:0a75456de360e6bdb884196a71cbbc5cedc0ec95b9cbd5c86a0861f8e3115c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.4.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-alpine`

```console
$ docker pull caddy@sha256:47fbe5354ee0e56faaab47d85cd0e212914290367b7815eaea9175387a081145
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
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:276530503290de9ae8be7471e975d5db1e0d286e99d48317b675cec03c7c2fca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.4.6-builder-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.4.6-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.4.6-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1`

```console
$ docker pull caddy@sha256:c7ed849ec0bccc9590c081c1feb962b488026451d6353742625c9d059596992e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64
	-	windows version 10.0.20348.587; amd64

### `caddy:2.5.0-beta.1` - linux; amd64

```console
$ docker pull caddy@sha256:bcede2ab0f45a70eac60e260088ea63657c89a0dc68fb7516040aa3862cb7120
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15281226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f65d2ad1bd1cdcaf90480f47941d1b9d3cd79a6c377eb7a1797fdd11afde75`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:13 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 05:58:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:16 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:16 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:16 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:16 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:16 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 05:58:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:18 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1138def552ee0eeabfad7f99cd241e68999f18261070a8b846ed8b714970d1`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 291.5 KB (291519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895041dd1e627dbe5debbe3ccef97db110d6ff4fc85f6d97397c948d30ca1c87`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8fc9316afa2bc657ab6fe290e9ba1888c992ac4774a4b3be13313f18725b01`  
		Last Modified: Tue, 29 Mar 2022 05:58:56 GMT  
		Size: 12.2 MB (12169213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7b98a130990e6ca95fbb2149ae073311e5e3832ecdadc67cd29cf942e49efe`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de91e531a9131919b9e754e515670577052e7cc9492983e98baa252930b24365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14451265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66fa15c81d6e0fdbb69a30cafb1f242d980e16b20c3c80de06705e4e9972c393`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:30:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:30:00 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:30:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:30:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:30:07 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:30:07 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:30:08 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:30:08 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:30:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:30:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:30:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:30:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:30:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:30:12 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:30:13 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:30:13 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:30:14 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a59d599e5cf36191b1eda6d65d7dca2a20d945b52caa7c04f8eb23a29c88c`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 291.7 KB (291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be419f9ab7f9bc25bac2e99fe6b7259e47611111452bcf387dbdb252aa12137`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c6c14f54ca6f502c0736c47d5a75ed49c34bfbf7afe638f1f870812fe5c42`  
		Last Modified: Tue, 29 Mar 2022 07:32:06 GMT  
		Size: 11.5 MB (11531649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981f057ad3f9958644cac7924ea81334aaa0c76bcc7e5a186e173cb1e5b33ebb`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:760182586a270f65f6ae733cb021768b6a24194b496d9049abb80754c0a9ff49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14232924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b430d36d28f2ac85c509dca2dcd0a8fdb8634b559490a90081990df47985232`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:30:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:30:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:30:28 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 22:30:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:30:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:30:35 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:30:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:30:36 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:30:36 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:30:37 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 22:30:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:30:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:30:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:30:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:30:40 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:30:41 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:30:41 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:30:42 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:30:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c2df20f77228856c20a052139f9a32147de6fa7e2db9bdbd894eb7fa9b943`  
		Last Modified: Tue, 29 Mar 2022 22:32:31 GMT  
		Size: 290.7 KB (290669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3589e6943b5326d1317e0a2969d4099a2a41a63d79149965f0e9359177833`  
		Last Modified: Tue, 29 Mar 2022 22:32:30 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b122b7cc8b070009e8dcdf59e36800a16a13894fffa4a34392fe391bcdcc1b`  
		Last Modified: Tue, 29 Mar 2022 22:32:38 GMT  
		Size: 11.5 MB (11511973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c381aab113c8cb5ee770c3c726c6ff5c10bc6210abcc9699b42cf5a8bda992`  
		Last Modified: Tue, 29 Mar 2022 22:32:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6843ae4e9394d661d8a433073819258169527655d7951e0e86f6c4b864ad6590
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14151549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:115deda3155a8af4acf31587058069bee8e1d73bdd35f897b07cfd1ea372c982`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:24:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:24:24 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 08:24:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:24:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:24:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:24:30 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:24:31 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:24:32 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:24:33 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 08:24:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:24:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:24:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:41 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:42 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:43 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:44 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b04940fdcd9cb77d235799bd68001a5180aa612fd4c50aa840940ea82b95de`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 291.3 KB (291304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef0e56e3268cf667da0f6cf5e10800748c888f98de71849a1212ee665da57ab`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 5.7 KB (5749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62f55966944253bb379e4eaa540552b036c6497864af3300e06aa46cfee314`  
		Last Modified: Tue, 29 Mar 2022 08:25:47 GMT  
		Size: 11.1 MB (11137995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb565fbf0ef10bbf2b8524fb3d5304c3e965d1a805eb37771af3a30f70e4073`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:845a5d94e27aafde1de4113f359603c5f2bc2bf43d14df55d1fb241c5e67af80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be9d99f3aa21b742ddf9e0bcd50040a8e3da028c93b55d1b90cd9acdf901bdd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:10:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:10:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:10:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:11:04 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:11:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:11:15 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:11:22 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:11:27 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:11:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:11:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:11:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:11:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:11:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:11:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:12:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:12:13 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:12:20 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:12:30 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:12:38 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:12:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e1be9956ea08450182368837a0552abfdfbcb482b0891b655993559e508d61`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 293.7 KB (293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfd1dd00b9e457999b59324db36ace0ae9c0b04b08ad78bca0ffc2efb2210f4`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6ec780e34a8da33bea9b2143c2f05c20c72c417442e77da351f81ad084cb65`  
		Last Modified: Tue, 29 Mar 2022 07:13:59 GMT  
		Size: 10.7 MB (10675673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc5e94588d483ed6a601dc8f0949e22a743eef7a8b3a89fd12b96d94c9ab6a7`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; s390x

```console
$ docker pull caddy@sha256:95d336f02d39a7f71322474ec3e8c19ad7d095713c867641b4f433eb0fd2a477
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14627739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:984624dd7fe4826c4337003baa208f6e5d637cb93853a0da41cbf578fc65d8e3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:04:20 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:04:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:04:21 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 09:04:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:24 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:24 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:24 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:24 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:25 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:25 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:26 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:26 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee7c8ba60122de161b5d68f7a6975166b397cfb9ebe16fd50b4386184db05be`  
		Last Modified: Tue, 29 Mar 2022 09:43:58 GMT  
		Size: 291.8 KB (291828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7c6b32624b795000ca5fb90d6329e82f344e3d188d1eb17b7f95bae7d03b9c`  
		Last Modified: Tue, 29 Mar 2022 09:44:02 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca37559faddac359a6ed3b63a1b633da3242ad85dd02a479d42d85eec3a21beb`  
		Last Modified: Tue, 29 Mar 2022 09:44:02 GMT  
		Size: 11.7 MB (11729491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ff24d1eb1ce2ce17f89047c855ddadc0723d0b0f623cc849c1b62661e9075d`  
		Last Modified: Tue, 29 Mar 2022 09:43:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:7773fd461ee6f12339ba1673bc5df75781a929c178c69f2b76f6dbb331c4b8a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728732764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1eacf7022523cf02e6baa380b984f1849385cfe6d35462401e39349c8fae5c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:15:55 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:17:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:17:02 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:17:03 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:17:05 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:17:06 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:17:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:17:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:17:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:17:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:17:24 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:17:26 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:17:28 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:18:46 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:18:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d7e8231020fca55f52d14b8a7ce3656ea1a0f7add52d65e90f62121fe48b8`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80d92ff4032a4af7c432751719331889e3987e12e65d34d5ebb282a20c93e9`  
		Last Modified: Thu, 10 Mar 2022 23:23:20 GMT  
		Size: 12.6 MB (12581604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3ae26f04e000ad3d59599134e362ac56f63587121dfd8c289ad4d7198b2c6`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe189798f275d20c78e39c5899fde1e4eb39b5215c94602a02494919622fbd1`  
		Last Modified: Thu, 10 Mar 2022 23:23:15 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bb6704511f5e25c596bb4da2e3876a4ff94d636a5a864cdc2081fa0c8c90e8`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60f4b9d1b8e2632e8c4b5a2ba5cef7b9d320a84cdc2f9b1602bf958c0eae59`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad4d74ac905f41961ea9c19da27a83ecf1f9e61f9f11698d8f6640f1ee42463`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c1b1b3adc2fba2aafe3fabc3589db5fee1a3e8804da41d5c86c57b9f715e34`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aeb6981196ccd526b2c147b65406c9e7ad753928b540d38b06ce826a10989`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9c3c1945a551d9fd87cdad01e126234fc6c19447c16283c1b7f3a9aaeaa85b`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fc2235c71cef450cb31287142ec7b1653b8aa10e4df09251c2fee9e45e9bfb`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1f868d3e6e3b7aeba72b31e537c64540b5cd47876b29dbc6b99449b042c77b`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1709c223988941e572100de0e0416fd946212338a4b82d0bf6157a0a9cffb`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31826e49182a6b827ba6af55bc08c92b46dcbd38b71dcfb68a76fa4b184624d`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bff2600becf937738dbbeabc119db87dc7bbf300de826c6f356cdf07824b4`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bd343b434eec8e57160a0b4c89e93ef67e08138859c36a8c46c14cbda37ca7`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14b1140f1d1c8b21f9bcd3ceb8f5dea64077c8d7cc78b9b4d9ed5b2f490cecd`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d5743206ba889ce28c20481d33002512a479d915ae0c5dfc5a8d01bbd943ed`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 307.8 KB (307825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f83df86e60e5b4e53108b5e0b1bf84a1c3bba826dd3ac59b4f7a1ac79a59908`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - windows version 10.0.20348.587; amd64

```console
$ docker pull caddy@sha256:190644b756f6e29fdd566242137d83a8ab8cb5da79c6eeb5a686acb280d0c87d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2234975577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec73698bb10b0a408086c4dd1fba649195a728ddf076a02f1e7367f9941183d0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:19:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:19:23 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:19:49 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:19:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:19:51 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:19:52 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:19:52 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:19:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:19:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:19:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:19:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:19:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:20:00 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:20:01 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:20:02 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:20:16 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:20:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501204225ae4faaf2054af787801c79f59cd7e6764ba27480f88314d662fe8db`  
		Last Modified: Thu, 10 Mar 2022 23:23:35 GMT  
		Size: 618.1 KB (618083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b161fdd7e1eff73e0b69b5a534a91cdc416dbc212d1d41e86ed77f1bbbb4b`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec81d9b42cee80d858fed2642eb9fceb14a85637d3107bdd77360697068f968`  
		Last Modified: Thu, 10 Mar 2022 23:23:37 GMT  
		Size: 12.8 MB (12770708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf78f158dbd631347c47fa0b4b35ed7c16f4c617befa9f52fbae491a4a2085b`  
		Last Modified: Thu, 10 Mar 2022 23:23:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddd79c99dbc6f4dbaf32b5704dc85064b5abb0d388adf5d061eaab0e37b5afa`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fdbdbcc0a58e8c38006e9b158adc19da95d85b019433828016eac93f2c03ba`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba8cfc63470c708385e8d8796cfeea6c650b82d68526bd52d26418ba8ef3a33`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc704f14d84f4cd4b9a956f79720b1fa2fed3455d75920ae21828dba48e0a15c`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7390fcba4513a938ed30807fc0a4f3dc62ec98c0c3a81070185b3332cba558d`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4a1b650b0b42f48eb9be5a49262e9d61983a217fa6b9cef5c1c4e8ea6037a1`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9efc512998552b2c0eb4fd62b04c41138f65d14796d706304028d70fbc6b30`  
		Last Modified: Thu, 10 Mar 2022 23:23:29 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05756c324de05267a5034909e0c59ce72d9f72b09fab332779f98cd3801f0232`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f983684908d82bbab9bbc2f115c19a1f78b5048872a5e54f8d3d208e89fb6`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b450029ff204db60d8023c9e526c38205aec114ab62d67351b1f19004b330`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18554b6031813cc80f8ba7e5e1df6f947821e1d1d0a6cab8e410f650209d86ae`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bfbc8f27994a32c626bcad31c573c825f23474b2d2167338ee0d35de1e6099`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9e9fb9ea227f0f6e8f513e977a1965a7de7aa0d22c26685a156828a8ebf06c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35636b68f6f3e0d03a7ba26fb4b136786e49e7a155fecbfd189ba95f4e6f42c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98050fbe661913690cee263b64e5c1defd894c209a4ac627acd69b806ba17e7a`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 314.3 KB (314344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2dc85353d3e550445d387372cf10180870b8aa3bdf523148585e354588bfb4`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-alpine`

```console
$ docker pull caddy@sha256:d945359af6c3f6f813961e06a10f8e1c5b863383551ccf51753a79d7e8c88a63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.0-beta.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:bcede2ab0f45a70eac60e260088ea63657c89a0dc68fb7516040aa3862cb7120
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15281226 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26f65d2ad1bd1cdcaf90480f47941d1b9d3cd79a6c377eb7a1797fdd11afde75`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:13 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 05:58:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:16 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:16 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:16 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:16 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:16 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:16 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 05:58:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:17 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:17 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:18 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1138def552ee0eeabfad7f99cd241e68999f18261070a8b846ed8b714970d1`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 291.5 KB (291519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895041dd1e627dbe5debbe3ccef97db110d6ff4fc85f6d97397c948d30ca1c87`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8fc9316afa2bc657ab6fe290e9ba1888c992ac4774a4b3be13313f18725b01`  
		Last Modified: Tue, 29 Mar 2022 05:58:56 GMT  
		Size: 12.2 MB (12169213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef7b98a130990e6ca95fbb2149ae073311e5e3832ecdadc67cd29cf942e49efe`  
		Last Modified: Tue, 29 Mar 2022 05:58:54 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:de91e531a9131919b9e754e515670577052e7cc9492983e98baa252930b24365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14451265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66fa15c81d6e0fdbb69a30cafb1f242d980e16b20c3c80de06705e4e9972c393`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:58 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:30:00 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:30:00 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:30:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:30:06 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:30:07 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:30:07 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:30:08 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:30:08 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:30:09 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:30:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:30:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:30:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:30:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:30:12 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:30:12 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:30:13 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:30:13 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:30:14 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:30:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204a59d599e5cf36191b1eda6d65d7dca2a20d945b52caa7c04f8eb23a29c88c`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 291.7 KB (291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be419f9ab7f9bc25bac2e99fe6b7259e47611111452bcf387dbdb252aa12137`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363c6c14f54ca6f502c0736c47d5a75ed49c34bfbf7afe638f1f870812fe5c42`  
		Last Modified: Tue, 29 Mar 2022 07:32:06 GMT  
		Size: 11.5 MB (11531649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981f057ad3f9958644cac7924ea81334aaa0c76bcc7e5a186e173cb1e5b33ebb`  
		Last Modified: Tue, 29 Mar 2022 07:31:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:760182586a270f65f6ae733cb021768b6a24194b496d9049abb80754c0a9ff49
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14232924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b430d36d28f2ac85c509dca2dcd0a8fdb8634b559490a90081990df47985232`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:28 GMT
ADD file:8c959b80e3661beea7b3468017b88897d981bf52ed43c074e7c87ecb753e9059 in / 
# Tue, 29 Mar 2022 02:13:28 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:30:26 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:30:28 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:30:28 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 22:30:33 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:30:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:30:35 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:30:35 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:30:36 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:30:36 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:30:37 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 22:30:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:30:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:30:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:30:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:30:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:30:40 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:30:41 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:30:41 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:30:42 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:30:42 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:22b1e5a07a97d7af6fdc335e3b3a975b73908fa19b084289c408a00814da0398`  
		Last Modified: Tue, 29 Mar 2022 02:15:28 GMT  
		Size: 2.4 MB (2424303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955c2df20f77228856c20a052139f9a32147de6fa7e2db9bdbd894eb7fa9b943`  
		Last Modified: Tue, 29 Mar 2022 22:32:31 GMT  
		Size: 290.7 KB (290669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3589e6943b5326d1317e0a2969d4099a2a41a63d79149965f0e9359177833`  
		Last Modified: Tue, 29 Mar 2022 22:32:30 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b122b7cc8b070009e8dcdf59e36800a16a13894fffa4a34392fe391bcdcc1b`  
		Last Modified: Tue, 29 Mar 2022 22:32:38 GMT  
		Size: 11.5 MB (11511973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c381aab113c8cb5ee770c3c726c6ff5c10bc6210abcc9699b42cf5a8bda992`  
		Last Modified: Tue, 29 Mar 2022 22:32:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:6843ae4e9394d661d8a433073819258169527655d7951e0e86f6c4b864ad6590
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14151549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:115deda3155a8af4acf31587058069bee8e1d73bdd35f897b07cfd1ea372c982`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:05 GMT
ADD file:24e8b04304ef91bbf949674909ccaf2c66e3dcd096c3c307a0510569eadf576f in / 
# Tue, 29 Mar 2022 00:40:05 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:24:23 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:24:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:24:24 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 08:24:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:24:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:24:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:24:30 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:24:31 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:24:32 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:24:33 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 08:24:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:24:35 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:24:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:41 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:42 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:43 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:44 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:80fa7f07ec7b717ec5f8e2717b91e3d659e129052ec3def2570a5674322688d9`  
		Last Modified: Tue, 29 Mar 2022 00:41:08 GMT  
		Size: 2.7 MB (2716347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01b04940fdcd9cb77d235799bd68001a5180aa612fd4c50aa840940ea82b95de`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 291.3 KB (291304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef0e56e3268cf667da0f6cf5e10800748c888f98de71849a1212ee665da57ab`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 5.7 KB (5749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f62f55966944253bb379e4eaa540552b036c6497864af3300e06aa46cfee314`  
		Last Modified: Tue, 29 Mar 2022 08:25:47 GMT  
		Size: 11.1 MB (11137995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb565fbf0ef10bbf2b8524fb3d5304c3e965d1a805eb37771af3a30f70e4073`  
		Last Modified: Tue, 29 Mar 2022 08:25:45 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:845a5d94e27aafde1de4113f359603c5f2bc2bf43d14df55d1fb241c5e67af80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1be9d99f3aa21b742ddf9e0bcd50040a8e3da028c93b55d1b90cd9acdf901bdd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:16:52 GMT
ADD file:9e7b65a431d59070abaadae56d9c3fc59c899af881939e4353b1f524b2bd5185 in / 
# Tue, 29 Mar 2022 00:16:55 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:10:24 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:10:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:10:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:10:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:11:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:11:04 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:11:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:11:15 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:11:22 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:11:27 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 07:11:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:11:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:11:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:11:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:11:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:11:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:12:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:12:13 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:12:20 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:12:30 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:12:38 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:12:44 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1c611bca4fa49cac5bc1e3826ad53fee85ed659d24bffcccd86c3f04be07339a`  
		Last Modified: Tue, 29 Mar 2022 00:18:26 GMT  
		Size: 2.8 MB (2811009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e1be9956ea08450182368837a0552abfdfbcb482b0891b655993559e508d61`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 293.7 KB (293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bfd1dd00b9e457999b59324db36ace0ae9c0b04b08ad78bca0ffc2efb2210f4`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc6ec780e34a8da33bea9b2143c2f05c20c72c417442e77da351f81ad084cb65`  
		Last Modified: Tue, 29 Mar 2022 07:13:59 GMT  
		Size: 10.7 MB (10675673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc5e94588d483ed6a601dc8f0949e22a743eef7a8b3a89fd12b96d94c9ab6a7`  
		Last Modified: Tue, 29 Mar 2022 07:13:57 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:95d336f02d39a7f71322474ec3e8c19ad7d095713c867641b4f433eb0fd2a477
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14627739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:984624dd7fe4826c4337003baa208f6e5d637cb93853a0da41cbf578fc65d8e3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:04:20 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:04:21 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:04:21 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 09:04:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:24 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:24 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:24 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:24 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:24 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:24 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:25 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:25 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:26 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:26 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ee7c8ba60122de161b5d68f7a6975166b397cfb9ebe16fd50b4386184db05be`  
		Last Modified: Tue, 29 Mar 2022 09:43:58 GMT  
		Size: 291.8 KB (291828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7c6b32624b795000ca5fb90d6329e82f344e3d188d1eb17b7f95bae7d03b9c`  
		Last Modified: Tue, 29 Mar 2022 09:44:02 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca37559faddac359a6ed3b63a1b633da3242ad85dd02a479d42d85eec3a21beb`  
		Last Modified: Tue, 29 Mar 2022 09:44:02 GMT  
		Size: 11.7 MB (11729491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ff24d1eb1ce2ce17f89047c855ddadc0723d0b0f623cc849c1b62661e9075d`  
		Last Modified: Tue, 29 Mar 2022 09:43:58 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder`

```console
$ docker pull caddy@sha256:ff1b80516329d8dafa119ab6ddf66ba10bee753534b14f0ff8b3f9f4a5d67b8c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64
	-	windows version 10.0.20348.587; amd64

### `caddy:2.5.0-beta.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:faeea9e503a8403915af0f2f814d612c9f7430286713bfc70239f208d38a0576
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896ef023a4cc2fa0f04f1e28f657c2a7e35b0fecffedaa0223a0f273a7f5b8da`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:30 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 30 Mar 2022 13:56:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e18d4db37bef98be5db53a080d5f39c1dc622392a2dc49acfe877a4639b6dd3`  
		Last Modified: Wed, 30 Mar 2022 13:57:06 GMT  
		Size: 1.2 MB (1245712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8712e2cfcca5075eed70b704d0c0069b9ed35edce73cbd396dc673106bbf40b6`  
		Last Modified: Wed, 30 Mar 2022 13:57:06 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1f9536788f7a6904a0ea7ae038d52c460c0fcb3115fc0180df7566dc9ad4cc8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68287115bf74108f9efe61ed1942c3f4911accb0a592968b4999964f3857194`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:34 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 19:48:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1e18e35b1632661f9bf91bdc19a4bc902ef76f9a2d9c0494bf40ac095e5173`  
		Last Modified: Tue, 29 Mar 2022 19:50:13 GMT  
		Size: 1.2 MB (1178519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c9eb4e1adcd6215f5ff1e7c7c1637dd1aa75b815815ea71e1bbab9de38a4e`  
		Last Modified: Tue, 29 Mar 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ecbc10f3f810710b018049c60fc8e6eee68603d6e143125d52c698049bfe4ab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422a80d5b1020e2f6ea922c1ee34808bfc55b24c0a0ca63811e610bd56c7c31d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:36:00 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 04:36:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:36:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:36:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e57ba208689f1e427c40a667a2cbf3edb416f56bcb0ccd9acf9d92ff64cf7ec`  
		Last Modified: Thu, 24 Mar 2022 04:37:37 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c01f8f1215d9923669ae5bfd5ff09d671cc335546f613cb8dc65185fce8f4d9`  
		Last Modified: Thu, 24 Mar 2022 04:37:36 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e03d21b158b53739152a61e319318968c01bb7f87b7b2ca75b4dfa81eebc14e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298230d91553e6791cd20293b4590be6d4c1f50bae2c1d1a73828b2f37963ff0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:07:05 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 12:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:07:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:07:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:07:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc1f36fe97759a3c941c9bbb783a066a205d6a7641df288c8e398cf745c0adf`  
		Last Modified: Thu, 24 Mar 2022 12:08:01 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42056a5405a9966a5c1873220813b7c5dfd11720c840128f601dd8591eb0871`  
		Last Modified: Thu, 24 Mar 2022 12:08:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:e483074a29e546b36e2203bf14bb58c153e5ff44e11e808abdfab6fa82e461c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944022d2960c692dc7335ab921050060ff9f7023e99a428263163792fc7c81ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:32:03 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 03:32:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:32:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:32:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:32:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be52f569cec212bde962ac7e9b67f50a0939d936c96865cea5e497eb040db36`  
		Last Modified: Thu, 24 Mar 2022 03:33:29 GMT  
		Size: 1.1 MB (1120845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b792fe773414624529314bb651b4cb7e8ec707a5be98b213dc5c2a52bd2a5`  
		Last Modified: Thu, 24 Mar 2022 03:33:29 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:751c88cf01a010bf45c7520dc7eeac57c3f3605f8f56e34f509d1ab50b277c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41593f9c1830f265972a420457d578e493521345a0e5241c20d8b85ad0f09d2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:09:04 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 30 Mar 2022 11:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:09:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:09:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:09:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727aaf4525e5e3c914709a8176edb2486d413b6aef45c66fd49e1eb931e16a3`  
		Last Modified: Wed, 30 Mar 2022 11:09:58 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e008688557ca2b630e6f2770e2faf6b9b8795f3283fc73afff3b93ebeed60c3`  
		Last Modified: Wed, 30 Mar 2022 11:09:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:0e7f812fa3e2ecc803dd4fb7b20a72dd1c75759ce49778f51ea9a5bd1719b22d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1badd557216606e841971ecc4296c63549a10a87cecd522cd7b7c2fa6c353d93`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:20:35 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:20:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:21:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:21:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281142ca6a15b21cfc34926357f799ac7c38783ca3875011b160c096c3229d65`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc359b64dd95e97e38c7d61691e76c179b77cc013db0f1076e98fe6bb7be82bc`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3c36ea4dbe6709a5c743097ec10680741b0e35b0e9d41b2b703ed388f6cb4`  
		Last Modified: Thu, 10 Mar 2022 23:23:44 GMT  
		Size: 1.7 MB (1666531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389f0b289a5870da81d3b2ef7f3c7d5b1fb87e5f103073f2f7698ecafbef39a`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - windows version 10.0.20348.587; amd64

```console
$ docker pull caddy@sha256:8a2e818f9a28bbd1dd99edd69a77b39ff9b5447b52226a98ab1aac9992f6ee29
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2395021082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69a46232eca5f0ad5b7c29ac6bba9315f92b55caaf663cdf7404af3383e1549c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:12:32 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:12:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:12:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:12:36 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:13:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:13:33 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:14:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:32:11 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:34:51 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:34:53 GMT
WORKDIR C:\go
# Thu, 10 Mar 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:21:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:21:50 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:21:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:22:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:22:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0159fc3ccac7854a42bd259b35d4a6482bc698865860892cf564a444b3c63`  
		Last Modified: Wed, 09 Mar 2022 14:03:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45aae60408220ac14736ec0b59de947d214ff276f074c4d716f9f2107b81671`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eec0ac452237f9eaa33ce02c78ae43641960a5cd004be40f1e99f8eda401f78`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b14ad7e0d74c6938398565f29103030d14231a39603cb3fef811fa8a55be4a`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8065b93123915e69465b4ba5e604b150fa39c4157166451453950874ce4dedf`  
		Last Modified: Wed, 09 Mar 2022 14:03:16 GMT  
		Size: 25.7 MB (25684294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce2ababcffd2ebaadd4d6756c1408d978cbb56bfb5fac29069bf777e6eee0fd`  
		Last Modified: Wed, 09 Mar 2022 14:03:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cd0da17ace6307cacfc21df261451fc8967bbefa8bea2f39da28a647dc391d`  
		Last Modified: Wed, 09 Mar 2022 14:03:04 GMT  
		Size: 512.4 KB (512354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42222c033855a8bddbeb67a0b4cff5b2999afd4119720ee7e4fe9f6c59756404`  
		Last Modified: Wed, 09 Mar 2022 14:11:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73cbf8abb1840e446af856b56aac5dd2a832cfe370e17f2ee7b4cbea84ee32d`  
		Last Modified: Wed, 09 Mar 2022 14:12:03 GMT  
		Size: 145.7 MB (145695821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d3ebd62db6d310f5584c9e38da9d33e106ef41c0fbfc4fe4f99031b01cf183`  
		Last Modified: Wed, 09 Mar 2022 14:11:16 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42907e59cd53434417a3cee16107b6fd3c9e583a7e92f403da1edc9c8881d5`  
		Last Modified: Thu, 10 Mar 2022 23:23:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dba9ee51310a6df87f204c28a7052ce8cfe8fe4054efe85de312fd9ebd0d2a`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90ed7f357bfb619820be785ff8397518d8b81f789fe33d1a458aa78a0b2c293`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaade4b90a730c916671b2dce519d031c74921051d042a36460fb347c4f0f43`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb19e6205c8bf8fb08f0d0c098c493b74d6a86d71667408aa1fe3f689c0d1f`  
		Last Modified: Thu, 10 Mar 2022 23:23:52 GMT  
		Size: 1.9 MB (1863109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cafb79352f1994a6c222b27e70e550375956842aa86e55ba656bcc19c61031`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-alpine`

```console
$ docker pull caddy@sha256:d3c330e404ff43e818584bdda859105ea03351da79ce5f54f63177f28ab4e080
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.0-beta.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:faeea9e503a8403915af0f2f814d612c9f7430286713bfc70239f208d38a0576
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:896ef023a4cc2fa0f04f1e28f657c2a7e35b0fecffedaa0223a0f273a7f5b8da`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:30 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 30 Mar 2022 13:56:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e18d4db37bef98be5db53a080d5f39c1dc622392a2dc49acfe877a4639b6dd3`  
		Last Modified: Wed, 30 Mar 2022 13:57:06 GMT  
		Size: 1.2 MB (1245712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8712e2cfcca5075eed70b704d0c0069b9ed35edce73cbd396dc673106bbf40b6`  
		Last Modified: Wed, 30 Mar 2022 13:57:06 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:1f9536788f7a6904a0ea7ae038d52c460c0fcb3115fc0180df7566dc9ad4cc8f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68287115bf74108f9efe61ed1942c3f4911accb0a592968b4999964f3857194`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:34 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 29 Mar 2022 19:48:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1e18e35b1632661f9bf91bdc19a4bc902ef76f9a2d9c0494bf40ac095e5173`  
		Last Modified: Tue, 29 Mar 2022 19:50:13 GMT  
		Size: 1.2 MB (1178519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c9eb4e1adcd6215f5ff1e7c7c1637dd1aa75b815815ea71e1bbab9de38a4e`  
		Last Modified: Tue, 29 Mar 2022 19:50:13 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:ecbc10f3f810710b018049c60fc8e6eee68603d6e143125d52c698049bfe4ab4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:422a80d5b1020e2f6ea922c1ee34808bfc55b24c0a0ca63811e610bd56c7c31d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:36:00 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 04:36:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:36:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:36:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:36:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e57ba208689f1e427c40a667a2cbf3edb416f56bcb0ccd9acf9d92ff64cf7ec`  
		Last Modified: Thu, 24 Mar 2022 04:37:37 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c01f8f1215d9923669ae5bfd5ff09d671cc335546f613cb8dc65185fce8f4d9`  
		Last Modified: Thu, 24 Mar 2022 04:37:36 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e03d21b158b53739152a61e319318968c01bb7f87b7b2ca75b4dfa81eebc14e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:298230d91553e6791cd20293b4590be6d4c1f50bae2c1d1a73828b2f37963ff0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:07:05 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 12:07:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:07:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:07:09 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:07:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc1f36fe97759a3c941c9bbb783a066a205d6a7641df288c8e398cf745c0adf`  
		Last Modified: Thu, 24 Mar 2022 12:08:01 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42056a5405a9966a5c1873220813b7c5dfd11720c840128f601dd8591eb0871`  
		Last Modified: Thu, 24 Mar 2022 12:08:01 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:e483074a29e546b36e2203bf14bb58c153e5ff44e11e808abdfab6fa82e461c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944022d2960c692dc7335ab921050060ff9f7023e99a428263163792fc7c81ff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:32:03 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 24 Mar 2022 03:32:09 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:32:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:32:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:32:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be52f569cec212bde962ac7e9b67f50a0939d936c96865cea5e497eb040db36`  
		Last Modified: Thu, 24 Mar 2022 03:33:29 GMT  
		Size: 1.1 MB (1120845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2b792fe773414624529314bb651b4cb7e8ec707a5be98b213dc5c2a52bd2a5`  
		Last Modified: Thu, 24 Mar 2022 03:33:29 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:751c88cf01a010bf45c7520dc7eeac57c3f3605f8f56e34f509d1ab50b277c36
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b41593f9c1830f265972a420457d578e493521345a0e5241c20d8b85ad0f09d2`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:09:04 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 30 Mar 2022 11:09:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:09:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:09:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:09:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8727aaf4525e5e3c914709a8176edb2486d413b6aef45c66fd49e1eb931e16a3`  
		Last Modified: Wed, 30 Mar 2022 11:09:58 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e008688557ca2b630e6f2770e2faf6b9b8795f3283fc73afff3b93ebeed60c3`  
		Last Modified: Wed, 30 Mar 2022 11:09:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1fe485f15ae043ddc06909eb0db4aa8908640744f4115d31550a8db0aaa727d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.5.0-beta.1-builder-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:0e7f812fa3e2ecc803dd4fb7b20a72dd1c75759ce49778f51ea9a5bd1719b22d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1badd557216606e841971ecc4296c63549a10a87cecd522cd7b7c2fa6c353d93`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:20:35 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:20:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:21:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:21:35 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281142ca6a15b21cfc34926357f799ac7c38783ca3875011b160c096c3229d65`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc359b64dd95e97e38c7d61691e76c179b77cc013db0f1076e98fe6bb7be82bc`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde3c36ea4dbe6709a5c743097ec10680741b0e35b0e9d41b2b703ed388f6cb4`  
		Last Modified: Thu, 10 Mar 2022 23:23:44 GMT  
		Size: 1.7 MB (1666531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b389f0b289a5870da81d3b2ef7f3c7d5b1fb87e5f103073f2f7698ecafbef39a`  
		Last Modified: Thu, 10 Mar 2022 23:23:43 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:500919c1c14c459428f3cb78c62243ea182dbd19bbf0f991c7d4074cf432fc3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `caddy:2.5.0-beta.1-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull caddy@sha256:8a2e818f9a28bbd1dd99edd69a77b39ff9b5447b52226a98ab1aac9992f6ee29
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2395021082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69a46232eca5f0ad5b7c29ac6bba9315f92b55caaf663cdf7404af3383e1549c`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:12:32 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:12:34 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:12:35 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:12:36 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:13:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:13:33 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:14:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:32:11 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:34:51 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:34:53 GMT
WORKDIR C:\go
# Thu, 10 Mar 2022 23:21:48 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:21:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:21:50 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:21:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:22:16 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:22:17 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f0159fc3ccac7854a42bd259b35d4a6482bc698865860892cf564a444b3c63`  
		Last Modified: Wed, 09 Mar 2022 14:03:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45aae60408220ac14736ec0b59de947d214ff276f074c4d716f9f2107b81671`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eec0ac452237f9eaa33ce02c78ae43641960a5cd004be40f1e99f8eda401f78`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b14ad7e0d74c6938398565f29103030d14231a39603cb3fef811fa8a55be4a`  
		Last Modified: Wed, 09 Mar 2022 14:03:09 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8065b93123915e69465b4ba5e604b150fa39c4157166451453950874ce4dedf`  
		Last Modified: Wed, 09 Mar 2022 14:03:16 GMT  
		Size: 25.7 MB (25684294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce2ababcffd2ebaadd4d6756c1408d978cbb56bfb5fac29069bf777e6eee0fd`  
		Last Modified: Wed, 09 Mar 2022 14:03:05 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cd0da17ace6307cacfc21df261451fc8967bbefa8bea2f39da28a647dc391d`  
		Last Modified: Wed, 09 Mar 2022 14:03:04 GMT  
		Size: 512.4 KB (512354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42222c033855a8bddbeb67a0b4cff5b2999afd4119720ee7e4fe9f6c59756404`  
		Last Modified: Wed, 09 Mar 2022 14:11:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73cbf8abb1840e446af856b56aac5dd2a832cfe370e17f2ee7b4cbea84ee32d`  
		Last Modified: Wed, 09 Mar 2022 14:12:03 GMT  
		Size: 145.7 MB (145695821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d3ebd62db6d310f5584c9e38da9d33e106ef41c0fbfc4fe4f99031b01cf183`  
		Last Modified: Wed, 09 Mar 2022 14:11:16 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af42907e59cd53434417a3cee16107b6fd3c9e583a7e92f403da1edc9c8881d5`  
		Last Modified: Thu, 10 Mar 2022 23:23:53 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dba9ee51310a6df87f204c28a7052ce8cfe8fe4054efe85de312fd9ebd0d2a`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d90ed7f357bfb619820be785ff8397518d8b81f789fe33d1a458aa78a0b2c293`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcaade4b90a730c916671b2dce519d031c74921051d042a36460fb347c4f0f43`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fb19e6205c8bf8fb08f0d0c098c493b74d6a86d71667408aa1fe3f689c0d1f`  
		Last Modified: Thu, 10 Mar 2022 23:23:52 GMT  
		Size: 1.9 MB (1863109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cafb79352f1994a6c222b27e70e550375956842aa86e55ba656bcc19c61031`  
		Last Modified: Thu, 10 Mar 2022 23:23:50 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore`

```console
$ docker pull caddy@sha256:2af9e1d7b943f0166cba6c938edd39f8dc7d04e21de4f1014ab341733e0be872
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2686; amd64
	-	windows version 10.0.20348.587; amd64

### `caddy:2.5.0-beta.1-windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:7773fd461ee6f12339ba1673bc5df75781a929c178c69f2b76f6dbb331c4b8a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728732764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1eacf7022523cf02e6baa380b984f1849385cfe6d35462401e39349c8fae5c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:15:55 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:17:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:17:02 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:17:03 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:17:05 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:17:06 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:17:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:17:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:17:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:17:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:17:24 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:17:26 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:17:28 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:18:46 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:18:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d7e8231020fca55f52d14b8a7ce3656ea1a0f7add52d65e90f62121fe48b8`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80d92ff4032a4af7c432751719331889e3987e12e65d34d5ebb282a20c93e9`  
		Last Modified: Thu, 10 Mar 2022 23:23:20 GMT  
		Size: 12.6 MB (12581604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3ae26f04e000ad3d59599134e362ac56f63587121dfd8c289ad4d7198b2c6`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe189798f275d20c78e39c5899fde1e4eb39b5215c94602a02494919622fbd1`  
		Last Modified: Thu, 10 Mar 2022 23:23:15 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bb6704511f5e25c596bb4da2e3876a4ff94d636a5a864cdc2081fa0c8c90e8`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60f4b9d1b8e2632e8c4b5a2ba5cef7b9d320a84cdc2f9b1602bf958c0eae59`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad4d74ac905f41961ea9c19da27a83ecf1f9e61f9f11698d8f6640f1ee42463`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c1b1b3adc2fba2aafe3fabc3589db5fee1a3e8804da41d5c86c57b9f715e34`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aeb6981196ccd526b2c147b65406c9e7ad753928b540d38b06ce826a10989`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9c3c1945a551d9fd87cdad01e126234fc6c19447c16283c1b7f3a9aaeaa85b`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fc2235c71cef450cb31287142ec7b1653b8aa10e4df09251c2fee9e45e9bfb`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1f868d3e6e3b7aeba72b31e537c64540b5cd47876b29dbc6b99449b042c77b`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1709c223988941e572100de0e0416fd946212338a4b82d0bf6157a0a9cffb`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31826e49182a6b827ba6af55bc08c92b46dcbd38b71dcfb68a76fa4b184624d`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bff2600becf937738dbbeabc119db87dc7bbf300de826c6f356cdf07824b4`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bd343b434eec8e57160a0b4c89e93ef67e08138859c36a8c46c14cbda37ca7`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14b1140f1d1c8b21f9bcd3ceb8f5dea64077c8d7cc78b9b4d9ed5b2f490cecd`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d5743206ba889ce28c20481d33002512a479d915ae0c5dfc5a8d01bbd943ed`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 307.8 KB (307825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f83df86e60e5b4e53108b5e0b1bf84a1c3bba826dd3ac59b4f7a1ac79a59908`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-windowsservercore` - windows version 10.0.20348.587; amd64

```console
$ docker pull caddy@sha256:190644b756f6e29fdd566242137d83a8ab8cb5da79c6eeb5a686acb280d0c87d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2234975577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec73698bb10b0a408086c4dd1fba649195a728ddf076a02f1e7367f9941183d0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:19:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:19:23 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:19:49 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:19:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:19:51 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:19:52 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:19:52 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:19:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:19:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:19:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:19:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:19:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:20:00 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:20:01 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:20:02 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:20:16 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:20:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501204225ae4faaf2054af787801c79f59cd7e6764ba27480f88314d662fe8db`  
		Last Modified: Thu, 10 Mar 2022 23:23:35 GMT  
		Size: 618.1 KB (618083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b161fdd7e1eff73e0b69b5a534a91cdc416dbc212d1d41e86ed77f1bbbb4b`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec81d9b42cee80d858fed2642eb9fceb14a85637d3107bdd77360697068f968`  
		Last Modified: Thu, 10 Mar 2022 23:23:37 GMT  
		Size: 12.8 MB (12770708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf78f158dbd631347c47fa0b4b35ed7c16f4c617befa9f52fbae491a4a2085b`  
		Last Modified: Thu, 10 Mar 2022 23:23:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddd79c99dbc6f4dbaf32b5704dc85064b5abb0d388adf5d061eaab0e37b5afa`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fdbdbcc0a58e8c38006e9b158adc19da95d85b019433828016eac93f2c03ba`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba8cfc63470c708385e8d8796cfeea6c650b82d68526bd52d26418ba8ef3a33`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc704f14d84f4cd4b9a956f79720b1fa2fed3455d75920ae21828dba48e0a15c`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7390fcba4513a938ed30807fc0a4f3dc62ec98c0c3a81070185b3332cba558d`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4a1b650b0b42f48eb9be5a49262e9d61983a217fa6b9cef5c1c4e8ea6037a1`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9efc512998552b2c0eb4fd62b04c41138f65d14796d706304028d70fbc6b30`  
		Last Modified: Thu, 10 Mar 2022 23:23:29 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05756c324de05267a5034909e0c59ce72d9f72b09fab332779f98cd3801f0232`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f983684908d82bbab9bbc2f115c19a1f78b5048872a5e54f8d3d208e89fb6`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b450029ff204db60d8023c9e526c38205aec114ab62d67351b1f19004b330`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18554b6031813cc80f8ba7e5e1df6f947821e1d1d0a6cab8e410f650209d86ae`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bfbc8f27994a32c626bcad31c573c825f23474b2d2167338ee0d35de1e6099`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9e9fb9ea227f0f6e8f513e977a1965a7de7aa0d22c26685a156828a8ebf06c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35636b68f6f3e0d03a7ba26fb4b136786e49e7a155fecbfd189ba95f4e6f42c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98050fbe661913690cee263b64e5c1defd894c209a4ac627acd69b806ba17e7a`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 314.3 KB (314344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2dc85353d3e550445d387372cf10180870b8aa3bdf523148585e354588bfb4`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:cb16b8aea224ac5fcac35beb9514f818332a1b46c4a99005974b2da915619d32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:2.5.0-beta.1-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:7773fd461ee6f12339ba1673bc5df75781a929c178c69f2b76f6dbb331c4b8a9
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728732764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c1eacf7022523cf02e6baa380b984f1849385cfe6d35462401e39349c8fae5c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:15:55 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:17:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:17:02 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:17:03 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:17:05 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:17:06 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:17:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:17:11 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:17:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:17:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:17:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:17:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:17:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:17:24 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:17:26 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:17:28 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:18:46 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:18:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd9d7e8231020fca55f52d14b8a7ce3656ea1a0f7add52d65e90f62121fe48b8`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80d92ff4032a4af7c432751719331889e3987e12e65d34d5ebb282a20c93e9`  
		Last Modified: Thu, 10 Mar 2022 23:23:20 GMT  
		Size: 12.6 MB (12581604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d3ae26f04e000ad3d59599134e362ac56f63587121dfd8c289ad4d7198b2c6`  
		Last Modified: Thu, 10 Mar 2022 23:23:16 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe189798f275d20c78e39c5899fde1e4eb39b5215c94602a02494919622fbd1`  
		Last Modified: Thu, 10 Mar 2022 23:23:15 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bb6704511f5e25c596bb4da2e3876a4ff94d636a5a864cdc2081fa0c8c90e8`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de60f4b9d1b8e2632e8c4b5a2ba5cef7b9d320a84cdc2f9b1602bf958c0eae59`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad4d74ac905f41961ea9c19da27a83ecf1f9e61f9f11698d8f6640f1ee42463`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c1b1b3adc2fba2aafe3fabc3589db5fee1a3e8804da41d5c86c57b9f715e34`  
		Last Modified: Thu, 10 Mar 2022 23:23:14 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920aeb6981196ccd526b2c147b65406c9e7ad753928b540d38b06ce826a10989`  
		Last Modified: Thu, 10 Mar 2022 23:23:13 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9c3c1945a551d9fd87cdad01e126234fc6c19447c16283c1b7f3a9aaeaa85b`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20fc2235c71cef450cb31287142ec7b1653b8aa10e4df09251c2fee9e45e9bfb`  
		Last Modified: Thu, 10 Mar 2022 23:23:12 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1f868d3e6e3b7aeba72b31e537c64540b5cd47876b29dbc6b99449b042c77b`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c1709c223988941e572100de0e0416fd946212338a4b82d0bf6157a0a9cffb`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31826e49182a6b827ba6af55bc08c92b46dcbd38b71dcfb68a76fa4b184624d`  
		Last Modified: Thu, 10 Mar 2022 23:23:11 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e10bff2600becf937738dbbeabc119db87dc7bbf300de826c6f356cdf07824b4`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39bd343b434eec8e57160a0b4c89e93ef67e08138859c36a8c46c14cbda37ca7`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14b1140f1d1c8b21f9bcd3ceb8f5dea64077c8d7cc78b9b4d9ed5b2f490cecd`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d5743206ba889ce28c20481d33002512a479d915ae0c5dfc5a8d01bbd943ed`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 307.8 KB (307825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f83df86e60e5b4e53108b5e0b1bf84a1c3bba826dd3ac59b4f7a1ac79a59908`  
		Last Modified: Thu, 10 Mar 2022 23:23:09 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:fa27c627b6079b5f944febb88fc9ff13eba0477d345ee00bc89682c6cd960c0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `caddy:2.5.0-beta.1-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull caddy@sha256:190644b756f6e29fdd566242137d83a8ab8cb5da79c6eeb5a686acb280d0c87d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2234975577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec73698bb10b0a408086c4dd1fba649195a728ddf076a02f1e7367f9941183d0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:19:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 10 Mar 2022 23:19:23 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 10 Mar 2022 23:19:49 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 10 Mar 2022 23:19:50 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 10 Mar 2022 23:19:51 GMT
VOLUME [c:/config]
# Thu, 10 Mar 2022 23:19:52 GMT
VOLUME [c:/data]
# Thu, 10 Mar 2022 23:19:52 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Thu, 10 Mar 2022 23:19:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 10 Mar 2022 23:19:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 10 Mar 2022 23:19:55 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 10 Mar 2022 23:19:56 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 10 Mar 2022 23:19:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 10 Mar 2022 23:19:58 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 10 Mar 2022 23:19:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 10 Mar 2022 23:20:00 GMT
EXPOSE 80
# Thu, 10 Mar 2022 23:20:01 GMT
EXPOSE 443
# Thu, 10 Mar 2022 23:20:02 GMT
EXPOSE 2019
# Thu, 10 Mar 2022 23:20:16 GMT
RUN caddy version
# Thu, 10 Mar 2022 23:20:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501204225ae4faaf2054af787801c79f59cd7e6764ba27480f88314d662fe8db`  
		Last Modified: Thu, 10 Mar 2022 23:23:35 GMT  
		Size: 618.1 KB (618083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1b161fdd7e1eff73e0b69b5a534a91cdc416dbc212d1d41e86ed77f1bbbb4b`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec81d9b42cee80d858fed2642eb9fceb14a85637d3107bdd77360697068f968`  
		Last Modified: Thu, 10 Mar 2022 23:23:37 GMT  
		Size: 12.8 MB (12770708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf78f158dbd631347c47fa0b4b35ed7c16f4c617befa9f52fbae491a4a2085b`  
		Last Modified: Thu, 10 Mar 2022 23:23:32 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddd79c99dbc6f4dbaf32b5704dc85064b5abb0d388adf5d061eaab0e37b5afa`  
		Last Modified: Thu, 10 Mar 2022 23:23:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7fdbdbcc0a58e8c38006e9b158adc19da95d85b019433828016eac93f2c03ba`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba8cfc63470c708385e8d8796cfeea6c650b82d68526bd52d26418ba8ef3a33`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc704f14d84f4cd4b9a956f79720b1fa2fed3455d75920ae21828dba48e0a15c`  
		Last Modified: Thu, 10 Mar 2022 23:23:31 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7390fcba4513a938ed30807fc0a4f3dc62ec98c0c3a81070185b3332cba558d`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4a1b650b0b42f48eb9be5a49262e9d61983a217fa6b9cef5c1c4e8ea6037a1`  
		Last Modified: Thu, 10 Mar 2022 23:23:30 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9efc512998552b2c0eb4fd62b04c41138f65d14796d706304028d70fbc6b30`  
		Last Modified: Thu, 10 Mar 2022 23:23:29 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05756c324de05267a5034909e0c59ce72d9f72b09fab332779f98cd3801f0232`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f983684908d82bbab9bbc2f115c19a1f78b5048872a5e54f8d3d208e89fb6`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b450029ff204db60d8023c9e526c38205aec114ab62d67351b1f19004b330`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18554b6031813cc80f8ba7e5e1df6f947821e1d1d0a6cab8e410f650209d86ae`  
		Last Modified: Thu, 10 Mar 2022 23:23:28 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bfbc8f27994a32c626bcad31c573c825f23474b2d2167338ee0d35de1e6099`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9e9fb9ea227f0f6e8f513e977a1965a7de7aa0d22c26685a156828a8ebf06c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35636b68f6f3e0d03a7ba26fb4b136786e49e7a155fecbfd189ba95f4e6f42c`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98050fbe661913690cee263b64e5c1defd894c209a4ac627acd69b806ba17e7a`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 314.3 KB (314344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2dc85353d3e550445d387372cf10180870b8aa3bdf523148585e354588bfb4`  
		Last Modified: Thu, 10 Mar 2022 23:23:26 GMT  
		Size: 1.4 KB (1368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:dd418a7216b6f833804da6b82fb215b7659f22ba7dd0196e201b2266dc2fd095
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
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:0a75456de360e6bdb884196a71cbbc5cedc0ec95b9cbd5c86a0861f8e3115c9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:47fbe5354ee0e56faaab47d85cd0e212914290367b7815eaea9175387a081145
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
$ docker pull caddy@sha256:684caa85e3a20dc427c6ab1648ac0675a3bc55bdbd9caedd608c5341119b5505
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121342188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e76447f0c092e300988c9c9b29764fe2b8118411a82b80f6e75bf21e5e615d4e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:38:44 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 08:38:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:38:45 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:43:35 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 08:45:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 08:45:36 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 08:45:36 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 08:45:37 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 08:45:37 GMT
WORKDIR /go
# Wed, 30 Mar 2022 13:56:22 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 13:56:22 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 13:56:22 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 13:56:23 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 13:56:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 13:56:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 13:56:25 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b494d572400cf4b26beff6a89af57b70fbc1d7a2c1aa7a0d7b67c756bdaed61`  
		Last Modified: Tue, 29 Mar 2022 08:48:36 GMT  
		Size: 272.0 KB (271969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623a0a71bae0ad42e563158693955153f07807709bdfc51c2d2eb87baf220ff4`  
		Last Modified: Tue, 29 Mar 2022 08:48:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ff514aa992605ed21198a53ceed0c47e8edb853676389315d8a6cef6c38c22`  
		Last Modified: Tue, 29 Mar 2022 08:49:59 GMT  
		Size: 110.2 MB (110187822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978df4263d9ad5678b6a602ace67e809da83893f1669f1723ba02c6a5bdbe1b7`  
		Last Modified: Tue, 29 Mar 2022 08:49:45 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7b5672f7cb85ab5135252c890d8588b3b6119def995a918548856fc0950fb4`  
		Last Modified: Wed, 30 Mar 2022 13:56:54 GMT  
		Size: 6.8 MB (6821457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e2df2c950c1e118da25951c59a757e0c195f21858976f77aa574dbec26ceb1b`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec8e71dd2f032868b49deb8234efa6ebf30cfa57d8a0cd5b7f0c71a2b233bf6`  
		Last Modified: Wed, 30 Mar 2022 13:56:53 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:3b65e4ace88f181e88d38888c2e7bf45ab2ea95d2a70d1aa9e260a7e37265b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115819432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66f23978f531de3d6637fd8f52ffd68708d73a8f566c332f38f8098827478041`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:32 GMT
ADD file:44acf536d487bec7f7bf16561f4ec90e60d4447b3cbabfeca66953c4491aabeb in / 
# Tue, 29 Mar 2022 00:49:33 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:40:30 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 07:40:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:40:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:48:57 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 07:52:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 07:52:15 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 07:52:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 07:52:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 07:52:18 GMT
WORKDIR /go
# Tue, 29 Mar 2022 19:48:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 29 Mar 2022 19:48:04 GMT
ENV XCADDY_VERSION=v0.2.1
# Tue, 29 Mar 2022 19:48:05 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 19:48:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 29 Mar 2022 19:48:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 29 Mar 2022 19:48:08 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 29 Mar 2022 19:48:09 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:84f033dabe5013c0dfae4263abd951011719d0a15adc3c7312c5be994deff030`  
		Last Modified: Tue, 29 Mar 2022 00:51:25 GMT  
		Size: 2.6 MB (2621943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:026b5f27b2698e668042c86dd2538d12d411867d83d2a9d9af230e055fe5a181`  
		Last Modified: Tue, 29 Mar 2022 07:57:23 GMT  
		Size: 272.1 KB (272137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0516ac9f12d388332faafff86659644eed1224227ceb75f6ce803e022d535e`  
		Last Modified: Tue, 29 Mar 2022 07:57:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a782b491ecfba149c412f8ad872bcfa7287e6a7caa6357cdcfbcb807c8da98f0`  
		Last Modified: Tue, 29 Mar 2022 08:01:44 GMT  
		Size: 105.1 MB (105068727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c866997cbd03bebd88e007f49e1a9487fd4ba581dfa2a4d85eff8629736d28`  
		Last Modified: Tue, 29 Mar 2022 08:00:34 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607471521c979ff3df274d2a499d8cdb7828e08615e4a430c0732444a298c53`  
		Last Modified: Tue, 29 Mar 2022 19:49:56 GMT  
		Size: 6.7 MB (6677400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38cc531d7dbc490a2d6e6a7000ff2d423828e739ab7213320c86a635cdfc3005`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 1.2 MB (1178510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceed9226afbdee75100b0fe36dc64b2212a63594d9d0cd2c83756c32f4cc37b2`  
		Last Modified: Tue, 29 Mar 2022 19:49:54 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:02f8b98f2d7f610839150ec7c8b2cb28303ae5b928a3c46827dba569edcd4cc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114681140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3173e35645f6e2df7cbb70ab3f0caa9e2e9d580c868b7323cbd4daa9fdf36a95`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:43:55 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:43:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:43:56 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:48:35 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 19:51:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 19:51:52 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 19:51:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 19:51:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 19:51:54 GMT
WORKDIR /go
# Thu, 24 Mar 2022 04:35:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 04:35:31 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 04:35:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 04:35:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 04:35:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 04:35:35 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331b3631dc9d8ace1881c2cb1c28eb266b0ec19c778721faa865e7bb38223ff6`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 271.1 KB (271107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac904122a78116e4100e90af49a2891c00345dbccfae86db8d59e7eb485212d1`  
		Last Modified: Wed, 23 Mar 2022 19:55:19 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eba6f0fdfa168bee61b63cce8a65b54fc5a493c16656abe13d65fb568c83352f`  
		Last Modified: Wed, 23 Mar 2022 21:39:45 GMT  
		Size: 104.9 MB (104853378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137658965282de05bacdac1471373fd69acaae9418ca2169e043327d833e27ca`  
		Last Modified: Wed, 23 Mar 2022 21:38:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52955aeb924042d48cdbb607de289b7457f6a5d6a0e9739931f61fdfe427f344`  
		Last Modified: Thu, 24 Mar 2022 04:37:20 GMT  
		Size: 6.0 MB (5952171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4014b68d35871bfdbe2e53206c7c5d4ced7c200ae0fcd28605f203330c4bfe1`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 1.2 MB (1176709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1fba897ff3f805fe40858af1887544e7fa2e99543c8410fbfb002a3a21ddaf8`  
		Last Modified: Thu, 24 Mar 2022 04:37:18 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:ea3dfbed453c77f5f75be7cb81c2ccee9dce3c65b654e8ef309dfe32b33652e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115485391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15729f70afc23409c5069a96dd3a3a35df28d19c5becc3bdc6dacc7c156a3777`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 24 Mar 2022 00:36:14 GMT
ADD file:30da1868f9f0555fb3e5223cd75cbf3c31760c1b6087f42d78abb08a8c5066ff in / 
# Thu, 24 Mar 2022 00:36:14 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 08:40:42 GMT
RUN apk add --no-cache ca-certificates
# Thu, 24 Mar 2022 09:03:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 24 Mar 2022 09:03:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:05:34 GMT
ENV GOLANG_VERSION=1.17.8
# Thu, 24 Mar 2022 09:06:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 24 Mar 2022 09:06:52 GMT
ENV GOPATH=/go
# Thu, 24 Mar 2022 09:06:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Mar 2022 09:06:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 24 Mar 2022 09:06:55 GMT
WORKDIR /go
# Thu, 24 Mar 2022 12:06:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 12:06:48 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 12:06:49 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 12:06:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 12:06:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 12:06:54 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 12:06:54 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a5e44472bb1f0d721d23f82fa10a4c3d25994790238a173c1de950a649eb9a90`  
		Last Modified: Wed, 23 Mar 2022 20:10:33 GMT  
		Size: 2.7 MB (2714720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b0b4c4587fbfa6f0755490bb53175932c8f0348926efd629b5e26b281aaa57`  
		Last Modified: Thu, 24 Mar 2022 08:41:08 GMT  
		Size: 271.8 KB (271767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63bc71a7e8dd1d9668121710be981aa07a74660d94ff3bc08a49ec70e7654c7f`  
		Last Modified: Thu, 24 Mar 2022 09:08:22 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f22eeb6ec86e713b0a2cb7da0cc984bba811a2fd1d3aef57ac8a509969f9a2e`  
		Last Modified: Thu, 24 Mar 2022 09:09:26 GMT  
		Size: 104.4 MB (104423565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1374803ba168889172986189f9d0d20f5b1491771af58ebe714cb84f99fa3a15`  
		Last Modified: Thu, 24 Mar 2022 09:09:11 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a9f8667a88f626fef41f02488af5fd79509d422aa4e00fe721fd704c067f87`  
		Last Modified: Thu, 24 Mar 2022 12:07:47 GMT  
		Size: 6.9 MB (6925978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44b55c23fcf50b7be62fd87f864eb47347cc2bffb823221798cbfcf40d994fdd`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d38bff84bce7d7ee9ea1a3bfe3473790a3681d0ecec05d0bdd077af8a567ab1`  
		Last Modified: Thu, 24 Mar 2022 12:07:46 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:11649bbf1cf06ebea3bcef630c8601cc35feaa553ade9923fa62f53c282db438
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114315662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc5080a9dc71d919e80a3f561c2b9af0560976209f3535b1c327b1f26650fff`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:57:35 GMT
RUN apk add --no-cache ca-certificates
# Wed, 23 Mar 2022 19:57:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 23 Mar 2022 19:57:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:14:48 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 23 Mar 2022 20:17:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 23 Mar 2022 20:17:23 GMT
ENV GOPATH=/go
# Wed, 23 Mar 2022 20:17:31 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 20:17:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 23 Mar 2022 20:17:52 GMT
WORKDIR /go
# Thu, 24 Mar 2022 03:31:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 24 Mar 2022 03:31:15 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 24 Mar 2022 03:31:18 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 24 Mar 2022 03:31:25 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 24 Mar 2022 03:31:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 24 Mar 2022 03:31:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 24 Mar 2022 03:31:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1638cef9b912d53eb425be9e028b98f20521ef09b221e120180e69b238a14321`  
		Last Modified: Wed, 23 Mar 2022 20:19:18 GMT  
		Size: 274.2 KB (274168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611046ca672b25224535bd7440ddf58c8b3f23db1f3b3a079dd7411ea06aafa1`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5277b684f884438c817309578480b4bbaf44dec0767ea8c51ceb76bb9b9b60`  
		Last Modified: Wed, 23 Mar 2022 20:19:35 GMT  
		Size: 102.8 MB (102784907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb475fbb9abdc19e3bb6e3ce9caedb03b0cfb03f91dffdc01117daa32d36dfa`  
		Last Modified: Wed, 23 Mar 2022 20:19:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cb43e7adeb1ac72bd05420bc8de466a4b23f7ef2834419cbbe6f04415022f1`  
		Last Modified: Thu, 24 Mar 2022 03:33:11 GMT  
		Size: 7.3 MB (7320988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c822ff2754104c9cdf880adb708e4dec3d253566eb6e2287220bab202d462abc`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 1.1 MB (1120846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016dbe0d502dc8e63e4f16f1f7936c74e076cbf990aaea69795c2a56b4c137df`  
		Last Modified: Thu, 24 Mar 2022 03:33:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cea02a6e6848170d0813a2356553deadab852697671d6269d83d23dedd4bbdce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118747209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df702fbf0389f742c73969d60ddeb12b5353892e9c405d0c921f000bea143f18`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:32 GMT
ADD file:75e6f1cb0cdf63de14d99f8419ce47d61e295300299c18b08bd484dff0da4e93 in / 
# Tue, 29 Mar 2022 00:41:32 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 10:03:25 GMT
RUN apk add --no-cache ca-certificates
# Tue, 29 Mar 2022 10:03:25 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 10:03:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:07:43 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 29 Mar 2022 10:09:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 29 Mar 2022 10:09:23 GMT
ENV GOPATH=/go
# Tue, 29 Mar 2022 10:09:24 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 29 Mar 2022 10:09:24 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 29 Mar 2022 10:09:24 GMT
WORKDIR /go
# Wed, 30 Mar 2022 11:08:48 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 30 Mar 2022 11:08:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 30 Mar 2022 11:08:49 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 30 Mar 2022 11:08:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 30 Mar 2022 11:08:50 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 30 Mar 2022 11:08:50 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:2c33ece150b7a4954636e49b807bdf240c422de7a78f45728d2fcdb7c96d14a3`  
		Last Modified: Tue, 29 Mar 2022 00:44:03 GMT  
		Size: 2.6 MB (2600441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ee16316d74aefe45b4279f488a09f3f5c4352904229634f9af35cfcec322bb`  
		Last Modified: Tue, 29 Mar 2022 10:13:07 GMT  
		Size: 272.3 KB (272277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8208057f374fb229f66af2db3ded59bcb907b24e1a83c4917138e1850638bcdb`  
		Last Modified: Tue, 29 Mar 2022 10:13:08 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b066059245d03bfd756f2c10ad89c93b0b6689c90d8f6bccfcfae7f3649d5761`  
		Last Modified: Tue, 29 Mar 2022 10:19:26 GMT  
		Size: 107.7 MB (107739123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34b5a23826dc3c170bc4eded13a252d4047906b3d697000e05ad3424410e1`  
		Last Modified: Tue, 29 Mar 2022 10:19:22 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b73fe01eaa3a41a15420b9b15f9e61572610d83447d6e9c7fbdb8c152dcaff`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 6.9 MB (6930870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2bce9e9a7094d845ec5bb32825d60ef6c2c62a6756606ba3cc8fb7a250f6`  
		Last Modified: Wed, 30 Mar 2022 11:09:47 GMT  
		Size: 1.2 MB (1203784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d55a197cfe92f3a7e96d635155081be27ce3af8077a6448530df3dabfe88e63`  
		Last Modified: Wed, 30 Mar 2022 11:09:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:276530503290de9ae8be7471e975d5db1e0d286e99d48317b675cec03c7c2fca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:568847e6f37af8e2f55d5d780b100e1dbfcbb9178896eb9d8f2b57ecf966d39c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888394051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20261b1174a82d98f801248da692dc2862f133c7cea9e52758b2c17b3567abc3`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 13:17:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 09 Mar 2022 13:17:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 09 Mar 2022 13:17:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 09 Mar 2022 13:17:28 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 09 Mar 2022 13:19:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:19:56 GMT
ENV GOPATH=C:\go
# Wed, 09 Mar 2022 13:20:52 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 13:35:10 GMT
ENV GOLANG_VERSION=1.17.8
# Wed, 09 Mar 2022 13:38:26 GMT
RUN $url = 'https://dl.google.com/go/go1.17.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '85ccf2608dca6ea9a46b6538c9e75e7cf2aebdf502379843b248e26b8bb110be'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 13:38:28 GMT
WORKDIR C:\go
# Wed, 09 Mar 2022 18:27:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 10 Mar 2022 23:14:28 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 10 Mar 2022 23:14:29 GMT
ENV CADDY_VERSION=v2.4.6
# Thu, 10 Mar 2022 23:14:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 10 Mar 2022 23:15:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 10 Mar 2022 23:15:41 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7705bbffd7dc00934e935de0e00e09a7b0da55d66c596622f094495478dd71`  
		Last Modified: Wed, 09 Mar 2022 14:04:13 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be7ff0bb187d149a5cf3c76e1ec444d0e07c6606f67b2c921c67ec91829ea03`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876223f25b257577440a80fdee021b43c33ce3c56be9a20b2ddeaede95240522`  
		Last Modified: Wed, 09 Mar 2022 14:04:12 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991eea244b9c3a1849c84748425dd9e9fbf9ec359ad9329796131b929239ffa4`  
		Last Modified: Wed, 09 Mar 2022 14:04:11 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b4c7c9740eb99bf626b312aa69396db3d186c5bd0e092b01c078ca7248e386`  
		Last Modified: Wed, 09 Mar 2022 14:04:40 GMT  
		Size: 25.5 MB (25454695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36f6c8a4d4848c21636a48a69a569a5372ec4890ea029f1f620dda76078bdcef`  
		Last Modified: Wed, 09 Mar 2022 14:04:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ac6d527939082add6d21652ba4888acc5a6e7607365168d8e61fb1485339cb`  
		Last Modified: Wed, 09 Mar 2022 14:04:10 GMT  
		Size: 313.6 KB (313592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37aeceb8c2e5bb3c500129bcf20c3f8aea8c68c353e6714a63a225ed1546e8a1`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d88cd595dc7580d72420b7288c52d4b32201045a13dda1a7b943d9a3468adef`  
		Last Modified: Wed, 09 Mar 2022 14:13:05 GMT  
		Size: 145.5 MB (145488847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be492983ee2b2c9128ce0c732c441ae5fbd203cdb71c94faa253c24b01750c90`  
		Last Modified: Wed, 09 Mar 2022 14:12:20 GMT  
		Size: 1.5 KB (1523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa7b09ca61eb1fbafacee427b430b0879ad4da23e62e430a3fe6a66f181f642`  
		Last Modified: Wed, 09 Mar 2022 18:30:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74014ffde8e1a1677cd81e965bcd2b1f5287bcbf682bbce3bdd125052cd04f29`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a43e7b3a6c47e8c9bba8e4ba91d722cd9e491f2df12d5e277356e2b8fc070ba8`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceffc29f93380b6942a245303d5af87875d60351e4c897405f358f018b61b863`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae9e05c08471d9a54c2b46c4f892226ab1eab63b6efd326c44b50bceffb11f2`  
		Last Modified: Thu, 10 Mar 2022 23:22:56 GMT  
		Size: 1.7 MB (1665933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd386d40eef8a252639d03e1486ff30ff8f77cef626bf0592cc7853eb633c7d`  
		Last Modified: Thu, 10 Mar 2022 23:22:54 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:f4840526af7bf068e5e8941e190bb42c0c8e98f10b2ee576d92ff85cba9d368d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2686; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:7351b0518db8c51c18809a4d43afd7903a465d3dca5c77da719c5cc7a81a1740
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0b2dfe5e74ccb861b7a35cbefe32c1c5e96acde70cddc38cf3d8f64d90deb13`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 05:58:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 05:58:02 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 05:58:02 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 05:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 05:58:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 05:58:05 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 05:58:05 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 05:58:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 05:58:06 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 80
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 443
# Tue, 29 Mar 2022 05:58:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 05:58:06 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 05:58:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16aa0ab1de725bc7131f63299135ba60863ca8149840ea4bd6df1f4f2d60889`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 291.2 KB (291224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1e6aebf4c6a6953bb272a1e9fbd9db3baa07a99ec49a86b1237cfdb8b2cbf`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3631b912ac5a3f1a6f50d287807d78710918b3b4ef93430ca5f92909b44d178`  
		Last Modified: Tue, 29 Mar 2022 05:58:41 GMT  
		Size: 11.7 MB (11726447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6f9dac281a690e38e3dc02f848e6bca3e352cc49e599982e4c5e1bd8c23653`  
		Last Modified: Tue, 29 Mar 2022 05:58:39 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:887a647096a6d56dcb36e25de7266207e84d8c6a16a6f3ea45bbd54980942676
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049436 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d253fe85a3c9b57835a6000f1fe71382ec9de663eac1ad339dacb903b187d92`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:29:07 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:29:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:29:10 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:29:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:29:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:29:17 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:29:18 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:29:18 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:29:19 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:29:19 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:29:20 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:29:21 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:29:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:29:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:29:23 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:29:24 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:29:25 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a57e26547e5eaa6e337f962fca1604a37c74bf6b9b212c1bc6d941ebdebac5c`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 291.6 KB (291643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52bbf90978f7165653e0da4087293508d6779069ccbc2d25a920a236b05c0ed6`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77ba24b9b18d0a95a2f6b7c8ad08aedf00cc0a8914556bb3ba92af3028279a4`  
		Last Modified: Tue, 29 Mar 2022 07:31:41 GMT  
		Size: 11.1 MB (11125794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1eaddacedb8aaf437331a7cf3feffa442e1d93dfb8cf857a9f30ea48820941b`  
		Last Modified: Tue, 29 Mar 2022 07:31:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:43c093b34865095ec01ba7ee64c3ff4399c351d253bbf5da810946e3cc2812e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831309 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5c0ddc24e3e17be6e36db8bcf57005e41e2b5f8569df67f954ec65b5371903`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 22:29:37 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 22:29:39 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 22:29:40 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 22:29:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 22:29:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 22:29:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 22:29:47 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 22:29:47 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 22:29:48 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 22:29:48 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 22:29:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 22:29:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 22:29:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 22:29:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 22:29:52 GMT
EXPOSE 80
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 443
# Tue, 29 Mar 2022 22:29:53 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 22:29:54 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 22:29:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237e0531178776616ebec915cc3eb77d92d704a49b39a5af3ee8abf41c0575c3`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b0acd6a99d4128b8e1364382254b31074a158bf903cd8b56800e1ffd0dd003b`  
		Last Modified: Tue, 29 Mar 2022 22:32:04 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db96e6a909b87d7b7978f48c12cd816e29760f854fcd6dd0280a247f8e6bcc49`  
		Last Modified: Tue, 29 Mar 2022 22:32:12 GMT  
		Size: 11.1 MB (11106725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be10db8a4481de128cefbde24b29a3c3f3328b2d5b2fcf2f3be5cc5439c5f8c`  
		Last Modified: Tue, 29 Mar 2022 22:32:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:27f7090978b59f3958bce30a9d3b41e4a08ef58ec35ab89a34660ca9eb101487
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57474591395abef876ba8baa368f50f88e62b9efd13497384ec14f9f096f22b6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 08:23:44 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 08:23:46 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 08:23:47 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 08:23:50 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 08:23:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 08:23:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 08:23:53 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 08:23:54 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 08:23:55 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 08:23:56 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 08:23:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 08:23:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 08:23:59 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 08:24:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 08:24:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 08:24:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 08:24:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 08:24:04 GMT
EXPOSE 80
# Tue, 29 Mar 2022 08:24:05 GMT
EXPOSE 443
# Tue, 29 Mar 2022 08:24:06 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 08:24:07 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 08:24:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bd3f5973f9a4dbe538674eed004edcfe5d94c3d62dc7ef4014e3ec8cc7b248`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 291.3 KB (291283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c471cc3b844311698bc73bb5f983caba3ffa244d5bb0dff7291722e9bbf2aeca`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60557a71741c85581eeb3297c963b0f83be72167076c5c26438a5b05ecba7e3`  
		Last Modified: Tue, 29 Mar 2022 08:25:28 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015cb2e22d3d113e599eb30d30a68280f3be03946b4255d32d81a6e0fb912017`  
		Last Modified: Tue, 29 Mar 2022 08:25:27 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:8a5bc601f4681d47af0376a9554ac1902679d567dcb0b153229173caafd15d11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1c8e3165344d7721d3317614b88868961a1dc50cf7bbdbb5868b44646b616a4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:08:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 07:08:12 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 07:08:17 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 07:08:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 07:08:38 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 07:08:43 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 07:08:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 07:08:50 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 07:08:53 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 07:08:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 07:09:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 07:09:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 07:09:12 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 07:09:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 07:09:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 07:09:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 07:09:36 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 07:09:39 GMT
EXPOSE 80
# Tue, 29 Mar 2022 07:09:44 GMT
EXPOSE 443
# Tue, 29 Mar 2022 07:09:48 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 07:09:52 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 07:09:57 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97dfd2f28bb7e55146245daf414143bb33d1cdc5e3635e545ae205d9694c288e`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 293.7 KB (293726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebfec2173c0a84f553475578ff76162e6ae96a2034405f90ee5cb03b62e51aa`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612c6f8ac456ea71d3eabf8534832fa947c011b2d8a205807b8575f7aacb6506`  
		Last Modified: Tue, 29 Mar 2022 07:13:40 GMT  
		Size: 10.3 MB (10302282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31728fd174d381d486cae7add3c74c79498390550a3f106832fe633b4b39cf6b`  
		Last Modified: Tue, 29 Mar 2022 07:13:38 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:6e9f4324a81f5d31d682b57b9abe53d70b5ff45ae11aa7e5b032ffad59d7e61b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a0b8d0b01eea60dfaa38989d8371165f6af04653867f53edaeba38d49c399f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 09:03:57 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 29 Mar 2022 09:03:58 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 29 Mar 2022 09:03:58 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 29 Mar 2022 09:04:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 29 Mar 2022 09:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 29 Mar 2022 09:04:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/config]
# Tue, 29 Mar 2022 09:04:02 GMT
VOLUME [/data]
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 29 Mar 2022 09:04:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 29 Mar 2022 09:04:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 80
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 443
# Tue, 29 Mar 2022 09:04:03 GMT
EXPOSE 2019
# Tue, 29 Mar 2022 09:04:03 GMT
WORKDIR /srv
# Tue, 29 Mar 2022 09:04:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b495e4184153b842af4cab4a18190da2a66c38474ea9cdbf35a598d9712f07`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 291.8 KB (291790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8239a2bbf380640e937ba02ea3c2e261571b2e5addb6baba61a6f2c3d39b2b9`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b93fd4ce47ae976a75a7bf38786bf8055d2516b14799d77742e9be41e81269d`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 11.3 MB (11323711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9ee986ce369a2c56741aaf75997532e7ec311362049f28e1d0dc7cd46261fc`  
		Last Modified: Tue, 29 Mar 2022 09:05:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:a3ba1d80239cc342421e0b3a6a6adba859191852e94c30047402f2ac1cc24407
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2686; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2686; amd64

```console
$ docker pull caddy@sha256:f2de2d90885f8cb6d12c79d914e354b41f6bfebc22ba3390096ae69fac380cf5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728251838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8705f493a3ce58fda2b9ada4d3d27639c9f13835f1fb8d85ecdf795e69dae46a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 19:31:54 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Mar 2022 18:20:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Mar 2022 18:20:27 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 09 Mar 2022 18:21:52 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Mar 2022 18:21:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Mar 2022 18:21:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Mar 2022 18:21:55 GMT
VOLUME [c:/config]
# Wed, 09 Mar 2022 18:21:56 GMT
VOLUME [c:/data]
# Wed, 09 Mar 2022 18:21:57 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 09 Mar 2022 18:21:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Mar 2022 18:21:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Mar 2022 18:22:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Mar 2022 18:22:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Mar 2022 18:22:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Mar 2022 18:22:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Mar 2022 18:22:05 GMT
EXPOSE 80
# Wed, 09 Mar 2022 18:22:06 GMT
EXPOSE 443
# Wed, 09 Mar 2022 18:22:07 GMT
EXPOSE 2019
# Wed, 09 Mar 2022 18:23:12 GMT
RUN caddy version
# Wed, 09 Mar 2022 18:23:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a42bef5ec276ee3f8dd3545bf050f4ab85c8191392884f5d5ad6af6ae6e2eed2`  
		Last Modified: Tue, 08 Mar 2022 20:01:19 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef99d892d6329e540cd98b358cc2f8085a7e6579538de9b4afa3ce0d11a03116`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 365.4 KB (365439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb2be6c676c8f3e743cd43ec6b238646cf9f8b89a6fb1bde29f9bb52a7296c`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9b968486191ed8bb4a6c85eb678e32bbb062d8998e636e7706431be6e25f51`  
		Last Modified: Wed, 09 Mar 2022 18:29:07 GMT  
		Size: 12.1 MB (12115400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63f0ecb87a49981ac55c8495d8beed3b58d3b15e31ff4ba1140b0176e551265`  
		Last Modified: Wed, 09 Mar 2022 18:29:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5249439459c9b885575d1a0c5c0df8c3e99649414b3c09ef4054e22fab54b584`  
		Last Modified: Wed, 09 Mar 2022 18:29:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69ab39aec279710b6bf7b4581cafe49878e70beff74d4a5e342eea02e60ce60`  
		Last Modified: Wed, 09 Mar 2022 18:29:02 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb81ca26c7a917813faca1d4cb92e1f41e642701d1199c9811ae8f9294e5b6f`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f5adb02b69cdd17e3acff1b0ea61317020c331399b0cb57fa34da5c09956e3`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e95a1158bc8e4066b6eb4211e7e898c86431c53c76c4752dfd7ce0a15cfc48`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579759f42b06baed2eb773c9cf8d6709e48e71afc07751fb3d45f7e4df9d819a`  
		Last Modified: Wed, 09 Mar 2022 18:29:01 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e477dc674aa75d9872e80416c27f642531913f63b1598f0920a821c8b6cb535c`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03c9bb84aaf51c973e2ae3990a6b45ac835195b5eaae35799354b2aee8dfc2e`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23add58da280a0f09c755eaccccd5ecc95dc65993558d933f499b4c3378c9f70`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e3da14e3fcc65b938eef87893e57b0daa81c012c8789265cd784fb2f3cfcf7`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34cb18e7475b74cb46643f516f65cbd77fa161c461d753b4e62e076f7b221e5`  
		Last Modified: Wed, 09 Mar 2022 18:28:59 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbd804e2eb98213ed819900a23753f3f2d662eb72c30a86dbbb51bcecc3cebc`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d49b05954d4ea193b3f85228739d529bbc2a811204d8b6e22440c97977addbdf`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a3a3abbfe3563eaed35b97ad1ed309a3f4e744f968d0b6f6deaf68211f2fc8`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53542589ba9c33b651da4be35de7384a168d4936d08bb046a632a4d644b46c9e`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 293.3 KB (293252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149ac7945e26171c6dfe9e316c21027eb072f4fd72819f8b80a32eada8275ae2`  
		Last Modified: Wed, 09 Mar 2022 18:28:57 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
