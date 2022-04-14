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
-	[`caddy:2.5.0-rc.1`](#caddy250-rc1)
-	[`caddy:2.5.0-rc.1-alpine`](#caddy250-rc1-alpine)
-	[`caddy:2.5.0-rc.1-builder`](#caddy250-rc1-builder)
-	[`caddy:2.5.0-rc.1-builder-alpine`](#caddy250-rc1-builder-alpine)
-	[`caddy:2.5.0-rc.1-builder-windowsservercore-1809`](#caddy250-rc1-builder-windowsservercore-1809)
-	[`caddy:2.5.0-rc.1-builder-windowsservercore-ltsc2022`](#caddy250-rc1-builder-windowsservercore-ltsc2022)
-	[`caddy:2.5.0-rc.1-windowsservercore`](#caddy250-rc1-windowsservercore)
-	[`caddy:2.5.0-rc.1-windowsservercore-1809`](#caddy250-rc1-windowsservercore-1809)
-	[`caddy:2.5.0-rc.1-windowsservercore-ltsc2022`](#caddy250-rc1-windowsservercore-ltsc2022)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)

## `caddy:2`

```console
$ docker pull caddy@sha256:53e1462eb68d51b5b2995be1c5d0c631fa67824f3fe37d692fe73ca714a7236f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:15e576e7d00b1f41a648c5295a03677c24da5fede09131edcb1e6d809c7dc8aa
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
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:c41bdf72cba4e0b7dea13a24c6a77d208ad4c56ba26ae6315e8b7298ee2911de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:b40a94d059874b25babe8cc3bf242e235761309e1454e9db7f36a0dd72bfa6b5
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
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4eed6304aa3dcd2487f2458eb28c35a51333b31ee8a245989fd6a72ab7d0ada6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6`

```console
$ docker pull caddy@sha256:53e1462eb68d51b5b2995be1c5d0c631fa67824f3fe37d692fe73ca714a7236f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.4.6` - linux; amd64

```console
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-alpine`

```console
$ docker pull caddy@sha256:15e576e7d00b1f41a648c5295a03677c24da5fede09131edcb1e6d809c7dc8aa
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
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder`

```console
$ docker pull caddy@sha256:c41bdf72cba4e0b7dea13a24c6a77d208ad4c56ba26ae6315e8b7298ee2911de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.4.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-alpine`

```console
$ docker pull caddy@sha256:b40a94d059874b25babe8cc3bf242e235761309e1454e9db7f36a0dd72bfa6b5
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
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4eed6304aa3dcd2487f2458eb28c35a51333b31ee8a245989fd6a72ab7d0ada6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.4.6-builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.4.6-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.4.6-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1`

```console
$ docker pull caddy@sha256:f61e24b2aed40d2f6f1c0520e54c9a8e0f9b787b1be2847712fe0d8f5642488d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-rc.1` - linux; amd64

```console
$ docker pull caddy@sha256:4c09cfec7af193d078894d0305810dbbe37d2079fc4e4aa0d15b2ba86b2a4e78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16764275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb962153761d3684fcdb4ba39f6194f56cb7bc50f315388d74d0c1847bdbd49b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:25:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:19:25 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:19:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:19:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:19:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:19:28 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:19:28 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:19:29 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:19:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840ff7bd6e2c9d7717705a52c1d27654581f987e1a43d2c9f3220ce850a5cdad`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031bccac710f69752f75ff47cd954b3b0a498c4d21cdf3d1d40d68fe2daf5111`  
		Last Modified: Thu, 14 Apr 2022 18:19:58 GMT  
		Size: 13.7 MB (13652213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb258af5a15a651f150eca21874b136e7fff707359f8dfc413238cfd95c87b`  
		Last Modified: Thu, 14 Apr 2022 18:19:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:8169a66902d5bc0166776d2ffc61a7cfe33e3524b45ae9d1f4b34832528e6aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16032265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6899c861932d4db0b1122cd039d86656c1be354bd5a00cf2878a3469d0db3ac0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:15:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:49:59 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:50:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:50:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:50:06 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:50:06 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:50:06 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:50:07 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:50:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:50:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:50:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:50:10 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:50:10 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:50:11 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:50:11 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:50:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac48280871fa0cc6e20550e9909af62acb5b3793a4ada967e49e60367ec386e`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85f1cf858fcca1ba11118dca6511d059f1dcc17491cbf5f798ea99c9e60395d`  
		Last Modified: Thu, 14 Apr 2022 18:51:55 GMT  
		Size: 13.1 MB (13112627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b3aa77c161606654441330d1170786a480ba08eb12e0fe4012bc22864d8cb`  
		Last Modified: Thu, 14 Apr 2022 18:51:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:010d0f2eacc275b3832b12f02e7c18db32f06d86fe332a5be38ecd0fc80c2d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15811406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd81531d9499cfff20362fecf182756c8be65dde798fa1f25e942af45cd72b67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:33:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:55:53 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:55:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:55:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:55:59 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:56:00 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:56:00 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:56:01 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:56:01 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:56:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:56:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:56:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:56:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:56:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:56:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:56:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:56:04 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:56:05 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:56:05 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:56:06 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:56:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2de87d2e387fcc410ddd706bbe177b2a04b5137087a6ffca70b45c80dc976e0`  
		Last Modified: Tue, 05 Apr 2022 06:35:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242051450e5651215542759d5d07707809ea50427c5b6de9c24d2480f2f6f8c4`  
		Last Modified: Thu, 14 Apr 2022 18:57:47 GMT  
		Size: 13.1 MB (13090432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1895805e4c28f2bf97a6ad0fe511d79ac99d357a44faa30cf6028762e5e2e3`  
		Last Modified: Thu, 14 Apr 2022 18:57:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:826ba1dc517fb61bf235692b48f85af8e61e39f99ba7ed75ff596f9ed9a81ba7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15502965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abdbc8e7155e22163727181dc120c2fc04f2aa4915a4e793f1e521816746c63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:12:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:39:42 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:39:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:39:47 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:39:48 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:39:49 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:39:50 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:39:51 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:39:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:39:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:39:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:39:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:39:59 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:40:00 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:40:01 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:40:02 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e87f72d84fd403dc0ea7d95672e5865925fca64a932f046b39035e8d3b43aae`  
		Last Modified: Tue, 05 Apr 2022 03:13:37 GMT  
		Size: 5.7 KB (5747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2191ecd11b5701c58e342cabfe4e55cb0cdab23c4d398594ab9f4bc9b41f8c2b`  
		Last Modified: Thu, 14 Apr 2022 18:40:54 GMT  
		Size: 12.5 MB (12489287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc6610077bf4a332f33ca9eda2d2fbefc8b8db78175b3cb0d450a1130bfd5e`  
		Last Modified: Thu, 14 Apr 2022 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:8c09a5c358d11a9907d3669e22520f753cab2a89b6285a66ff963f8dbc21d086
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15183296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6119f57d09c6c36ac71413249ac3c4104b9371f23a61c414de95458f2472d0c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:08:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 19:17:00 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:17:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 19:17:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 19:17:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 19:17:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 19:17:21 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 19:17:25 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 19:17:28 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:17:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:17:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:17:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:17:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:17:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:17:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:17:59 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:18:03 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:18:07 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:18:14 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 19:18:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029325992e21f613a5b486751627c7d5e5c7622ec29d4d170549f4dac13ad291`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faae2939aac44260ee51bef029b9e84eef0f871dccef0d5af41d2571dc9dc227`  
		Last Modified: Thu, 14 Apr 2022 19:19:29 GMT  
		Size: 12.1 MB (12072407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14abf82f7ea99e17942278eaaaa568df7b5ea903e8d5f5b3f1a4bf39c30b4c5`  
		Last Modified: Thu, 14 Apr 2022 19:19:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - linux; s390x

```console
$ docker pull caddy@sha256:2da1e6dd323af6077645f07f8d435d9248521aa41cb1ee22029d53f9a6910987
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16102259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff58a8f822ac8dbfcb3df4c5e34bea8d237836273a6e628764d82bb0ce89628a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:41:43 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:41:47 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:41:48 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:41:49 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:41:49 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:41:50 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:41:50 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:41:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36f8e9524a50422cbb86b1c5e3af26710e4b65591ecc118a5079f1aa7fe5a67`  
		Last Modified: Tue, 05 Apr 2022 06:20:45 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c0753886c9dbe469facec0509930b8dc3d42f92b0c579193f9d09927e092ee`  
		Last Modified: Thu, 14 Apr 2022 18:42:45 GMT  
		Size: 13.2 MB (13204080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1473aa5dc9f497cb2181788f19aae5e348c18f0393863acb9d8582c9a81eb73b`  
		Last Modified: Thu, 14 Apr 2022 18:42:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:7b19b5e3e5e35dde6a6cccda23e08c5c85cf68721e7bef80738dd82d935b1b16
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2730640494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ffd5b6e5907cb60d7a5adb0c56dc9053176223ecbf2bf5fcff3399f5f49e0f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:14:49 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:16:18 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:16:19 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:16:20 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:16:21 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:16:22 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:16:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:16:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:16:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:16:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:16:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:16:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:16:29 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:16:30 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:16:31 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:17:24 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12da94364e01a36d779bfafc8863ca1f7bf8234ce6f24988f68d1fd00ee02e06`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8ad753593036d1913b13edebd4355a905b469d0a9620d971dc9715f86e8ea2`  
		Last Modified: Thu, 14 Apr 2022 19:22:43 GMT  
		Size: 14.0 MB (13996925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c46084e73c5bf425af70578d2b0c76fabdccb126bc44c08c416817c1b6afe9c`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15af6c7018758c35ce48abb844810310bc64a68a6652695fc2de9b22707776b`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a6e7263b523e92d854d0cc0b89aadce4caeacc6525564cec3c2571bd621cd`  
		Last Modified: Thu, 14 Apr 2022 19:22:38 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04936128e7337a3425482423730fa939d21156c82597e0a3590049ed0a2fde57`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29420237ea837193935f4775de4cde39f9f998736b5298de43e472020d1d71df`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c94746d51b500baa19679f8aea92c90c46f6cac1d3040961911118da7432c1`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e02a7405a7e431869559ca1835268f104d17cc01aef969b01ce7929db2a5a5`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8372ff9d2fac7726f43c23f9c7f476ffd605f83ba9620d249300acf8607c2db`  
		Last Modified: Thu, 14 Apr 2022 19:22:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8b5f63b11c418280546ef6ed46310b89e4278ba33166610d216c24972be24`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a09cab4711bf91a1a3a3748a4c71bd78e41e199e554cc9a7c4173bcbe5c8515`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ce147cef3583f85a61794253d22dda5c99730a5b9362f69f2b40fe5baf7d34`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08658cd1da7ac20abe49b3609c5409267fcf83f9f14d854b6b72507b466ce003`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbdbe95ffca8c3113ef88ec04d897761f94fe44c70bc1d7bec368990ad24a6`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb5a4353c7ad939cf38f5f9e00cc9bd752ad926af8c9616942abdc79c3363`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4100dac27cedd92e1030d8b5a435307675c7c8f43b30b3b7a5d7a39ca8ff0f3c`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afafdaac1485785c781de040ff6901dde99b21ed257731f05118bab0c5955cc8`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 319.6 KB (319620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f2db279cae21b2def39302565eeb754e2903fae000c7dcf515d116a6c95aea`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:eb507596ef94e6ed3084201996e9f08e25b8745151ee6bedb7d36948dac054c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2242203268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffb97fd117fc020226f103385f120ef0e4e196a279809be3d26b3312a1f76bb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:45:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:17:36 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:18:44 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:18:45 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:18:46 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:18:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:18:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:18:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:18:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:18:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:18:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:18:54 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:18:55 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:18:56 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:19:30 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:19:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ff8ee97053f0fd2c04d1416858c55ed3909995cfc0831aa8f5a40204afd05`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 638.3 KB (638318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357652fda2b1e4d70c62d8d4ba35b476e36dd760b13a3eeacb8226bb50f448a`  
		Last Modified: Thu, 14 Apr 2022 19:22:57 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d217fa02930e4a656c7c4400fd7bb8baf3fa5702845f7e001de598bb9897c1`  
		Last Modified: Thu, 14 Apr 2022 19:23:00 GMT  
		Size: 14.2 MB (14225960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be5ff6bcf52b91e81fc414154427fb0320f1abcfe6cd53291f7b76a3f19cedb`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2215b48dac38251ea50b99034b6ccdbe83b2b4ab6a5e8476ae420eb6ea1507d6`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb351741bf0e672fb7c17e72bec00805d65311f8735a27cd33c428fd8c7db75`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ca0a8ec5cf1007e5e10a1d84ad67ed62967011eeaa10651e4df6599894d25`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978b105b9f03fa4b576a81dcef90374cb71c060548775a02686c100f1f9760e`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4840ed0bb6147c09215fa024ceb9fb9ec6638b7e05f03fde0c65345bc01257`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67111082235827f0f88e06d275ae8b7e1921e9d97e1cbe06b823ee7ad5670aff`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f9d794f6ff120d428bdc2cc5dcaa92736efe0cf104fbf7895e0a9bc4d0fac8`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175c2dc51ad06867c5059b438053a3806f5ef00aca3b9571c5b97db4aaecdf4`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623f3d22cd9cbdce94520c24cfac311df3e812b677cb5f16987daf5c00b923b`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f4acb76ece48c3ce666ca49abc7a0272959e573fad0222118435a37500fe0`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15acc8553457ab93836f3baa7faca6c62d13191114808e6c88d1c0dcd260307`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f336f0884a81040c8d84becf06b03a72aa1c1db7d627776ebc31681d037a08`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06694bc95a3b5673379a452023fab263afce2e02f3f735b3536478cb542f27e3`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38101d9aa2a7c4427ddc00488619fefd9ee139d7a3523644372beb8e5e95f7`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e25c0f33c7d9786bd26a0bf0d32451d9752eccab24b5cc2089a624c72efeff`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 358.7 KB (358693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ecdd10190bfd15bfb6eda278d94f8f29aadab7210e25a8ea1dbce0a60bd62`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-alpine`

```console
$ docker pull caddy@sha256:5e9ab55753068184099cdf778b4091be6ccb3229f5c5b4af41599af26bec4ed2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.0-rc.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:4c09cfec7af193d078894d0305810dbbe37d2079fc4e4aa0d15b2ba86b2a4e78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16764275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb962153761d3684fcdb4ba39f6194f56cb7bc50f315388d74d0c1847bdbd49b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:25:00 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:25:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:19:25 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:19:28 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:19:28 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:19:28 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:19:28 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:19:28 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:19:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:19:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:19:29 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:19:29 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:19:29 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87ed6b8c4412bcd2bb1f40611012b40444b12071baf4884d0e75044fc1f32c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 291.5 KB (291522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840ff7bd6e2c9d7717705a52c1d27654581f987e1a43d2c9f3220ce850a5cdad`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:031bccac710f69752f75ff47cd954b3b0a498c4d21cdf3d1d40d68fe2daf5111`  
		Last Modified: Thu, 14 Apr 2022 18:19:58 GMT  
		Size: 13.7 MB (13652213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:decb258af5a15a651f150eca21874b136e7fff707359f8dfc413238cfd95c87b`  
		Last Modified: Thu, 14 Apr 2022 18:19:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:8169a66902d5bc0166776d2ffc61a7cfe33e3524b45ae9d1f4b34832528e6aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (16032265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6899c861932d4db0b1122cd039d86656c1be354bd5a00cf2878a3469d0db3ac0`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:15:01 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:15:03 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:49:59 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:50:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:50:05 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:50:06 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:50:06 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:50:06 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:50:07 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:50:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:50:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:50:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:50:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:50:10 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:50:10 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:50:11 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:50:11 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:50:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52b230dd773e10769a2eb3e507260d2470a646efd48a639739ba8852b2915302`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 291.7 KB (291685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac48280871fa0cc6e20550e9909af62acb5b3793a4ada967e49e60367ec386e`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85f1cf858fcca1ba11118dca6511d059f1dcc17491cbf5f798ea99c9e60395d`  
		Last Modified: Thu, 14 Apr 2022 18:51:55 GMT  
		Size: 13.1 MB (13112627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d9b3aa77c161606654441330d1170786a480ba08eb12e0fe4012bc22864d8cb`  
		Last Modified: Thu, 14 Apr 2022 18:51:46 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:010d0f2eacc275b3832b12f02e7c18db32f06d86fe332a5be38ecd0fc80c2d15
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.8 MB (15811406 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd81531d9499cfff20362fecf182756c8be65dde798fa1f25e942af45cd72b67`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:33:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:33:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:55:53 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:55:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:55:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:55:59 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:56:00 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:56:00 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:56:01 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:56:01 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:56:01 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:56:02 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:56:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:56:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:56:03 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:56:04 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:56:04 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:56:04 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:56:05 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:56:05 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:56:06 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:56:06 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03203881a2568530a735b6e0e7a40ebb79adedc5193a675807b04eeb92cc6ed1`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 290.7 KB (290668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2de87d2e387fcc410ddd706bbe177b2a04b5137087a6ffca70b45c80dc976e0`  
		Last Modified: Tue, 05 Apr 2022 06:35:08 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242051450e5651215542759d5d07707809ea50427c5b6de9c24d2480f2f6f8c4`  
		Last Modified: Thu, 14 Apr 2022 18:57:47 GMT  
		Size: 13.1 MB (13090432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e1895805e4c28f2bf97a6ad0fe511d79ac99d357a44faa30cf6028762e5e2e3`  
		Last Modified: Thu, 14 Apr 2022 18:57:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:826ba1dc517fb61bf235692b48f85af8e61e39f99ba7ed75ff596f9ed9a81ba7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.5 MB (15502965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5abdbc8e7155e22163727181dc120c2fc04f2aa4915a4e793f1e521816746c63`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:12:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:39:42 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:39:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:39:46 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:39:47 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:39:48 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:39:49 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:39:50 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:39:51 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:39:52 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:39:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:39:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:39:58 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:39:59 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:40:00 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:40:01 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:40:02 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83aa37f2341b1e6d98420668c9bc849a47f2c471d159b2303885040bd8d0a92f`  
		Last Modified: Tue, 05 Apr 2022 03:13:38 GMT  
		Size: 291.3 KB (291301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e87f72d84fd403dc0ea7d95672e5865925fca64a932f046b39035e8d3b43aae`  
		Last Modified: Tue, 05 Apr 2022 03:13:37 GMT  
		Size: 5.7 KB (5747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2191ecd11b5701c58e342cabfe4e55cb0cdab23c4d398594ab9f4bc9b41f8c2b`  
		Last Modified: Thu, 14 Apr 2022 18:40:54 GMT  
		Size: 12.5 MB (12489287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fbc6610077bf4a332f33ca9eda2d2fbefc8b8db78175b3cb0d450a1130bfd5e`  
		Last Modified: Thu, 14 Apr 2022 18:40:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:8c09a5c358d11a9907d3669e22520f753cab2a89b6285a66ff963f8dbc21d086
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.2 MB (15183296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6119f57d09c6c36ac71413249ac3c4104b9371f23a61c414de95458f2472d0c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:08:34 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:08:43 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 19:17:00 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:17:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 19:17:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 19:17:16 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 19:17:19 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 19:17:21 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 19:17:25 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 19:17:28 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:17:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:17:33 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:17:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:17:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:17:47 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:17:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:17:54 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:17:59 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:18:03 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:18:07 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:18:14 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 19:18:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743509d6ced044a369685ebb068417e8757981a39d1b397c7b0182ab89f83528`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 293.7 KB (293721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029325992e21f613a5b486751627c7d5e5c7622ec29d4d170549f4dac13ad291`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faae2939aac44260ee51bef029b9e84eef0f871dccef0d5af41d2571dc9dc227`  
		Last Modified: Thu, 14 Apr 2022 19:19:29 GMT  
		Size: 12.1 MB (12072407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b14abf82f7ea99e17942278eaaaa568df7b5ea903e8d5f5b3f1a4bf39c30b4c5`  
		Last Modified: Thu, 14 Apr 2022 19:19:26 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2da1e6dd323af6077645f07f8d435d9248521aa41cb1ee22029d53f9a6910987
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16102259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff58a8f822ac8dbfcb3df4c5e34bea8d237836273a6e628764d82bb0ce89628a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:42 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Thu, 14 Apr 2022 18:41:43 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='e582db6dbc9a2c91c8d63d8c1376ec89929cafd731c6c53c6aa3f891afc7fe3276963900571a2eb10e77d19109f5e6734c64e70bea85b174e4530fac366cc6cc' ;; 		armhf)   binArch='armv6'; checksum='cd72e4bf741b424b58c5e19e9626110241bd728cf9426efd03089757c8e551bd50c473b07476f4b4130029838d62bdc0165a1e8ff5c0382de750f8217311cedf' ;; 		armv7)   binArch='armv7'; checksum='6351c947c340916f87789a65649322d537be2949003d679d19900af8e44ab6d0c15918938b7bdd022ff748a3d587d5c7f42d2d5310ef3fd49961b4382af77820' ;; 		aarch64) binArch='arm64'; checksum='e4697334cc01743b12f9ef3338923a5b8a4d51c17fc701d685d4a281f667a1a2378496d9567588ef7c01de3350eabf04455370f19620099b6f1cec6abf2ae54f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='3c4950414ae1b30e230f5766403ce0186f8e3badce8c097d54278df9ff942adfeffc845765d6d70a5d0d3352d548f2bfd346adfecb3dfa2e6903437aaf8bf0ba' ;; 		s390x)   binArch='s390x'; checksum='37cdd2e135760e2d9f58c47ed68b3575d281b0b710a70764cd27043f26ede076f2c3861c870546ecd931af23e6357a5cb87b52ec64ab7e5983e7a837a3131eb7' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 14 Apr 2022 18:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 14 Apr 2022 18:41:47 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 14 Apr 2022 18:41:47 GMT
ENV XDG_DATA_HOME=/data
# Thu, 14 Apr 2022 18:41:47 GMT
VOLUME [/config]
# Thu, 14 Apr 2022 18:41:48 GMT
VOLUME [/data]
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 18:41:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 18:41:49 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 18:41:49 GMT
EXPOSE 80
# Thu, 14 Apr 2022 18:41:49 GMT
EXPOSE 443
# Thu, 14 Apr 2022 18:41:50 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 18:41:50 GMT
WORKDIR /srv
# Thu, 14 Apr 2022 18:41:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8cc7c7c7ffd67f5740add448d341753330a2abdc6ed06e995cb7d28de381ab`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 291.8 KB (291821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36f8e9524a50422cbb86b1c5e3af26710e4b65591ecc118a5079f1aa7fe5a67`  
		Last Modified: Tue, 05 Apr 2022 06:20:45 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c0753886c9dbe469facec0509930b8dc3d42f92b0c579193f9d09927e092ee`  
		Last Modified: Thu, 14 Apr 2022 18:42:45 GMT  
		Size: 13.2 MB (13204080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1473aa5dc9f497cb2181788f19aae5e348c18f0393863acb9d8582c9a81eb73b`  
		Last Modified: Thu, 14 Apr 2022 18:42:43 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-builder`

```console
$ docker pull caddy@sha256:70884639bfbe324af8a10eab9b59fd395bcecadc32defa55f2478ef5f3db13f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-rc.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:39f14f117c0b3b4231d479b39592c96fe51d84503489ca70d2d6213b73b1371f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126725956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5332e4589600d01eb51e2690698aa0b12d8bcaf376e43b54be72b9f6f0ce913`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:20:33 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 02:34:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 02:34:25 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 02:34:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 02:34:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 02:34:25 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:19:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:19:34 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:19:34 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:19:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:19:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:19:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6858aa20941bdfe0d406b2e4db477feeccf42ca6e40478043b721c6a66f9d1b6`  
		Last Modified: Thu, 14 Apr 2022 02:37:21 GMT  
		Size: 115.6 MB (115569906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8029b02d49777774618d41ab3a1f7f4f32f7d4b10453afd26a184b8787beaa`  
		Last Modified: Thu, 14 Apr 2022 02:37:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852fa41bd6ab92e973a3316d6db4a27e9b1844abac8363c94c241958de8ad22`  
		Last Modified: Thu, 14 Apr 2022 18:20:07 GMT  
		Size: 6.8 MB (6823100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8824e5886ff61d400983eba90a9e3fd8fff37ed666dc3fbf532fb19336de59f0`  
		Last Modified: Thu, 14 Apr 2022 18:20:06 GMT  
		Size: 1.2 MB (1245713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935ac112e2d54d80c0e13be0791314cff9e6b1bec42d9354f90ff9c6bfedce2a`  
		Last Modified: Thu, 14 Apr 2022 18:20:06 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:638fe015b430dbd80bce39acaac9474eeef1183ca69eccba20942cbe5f7b62ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122713231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1ec6719298af0eae4e8c888c1a237942d068f190bda4b72fa419c9e9667080`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:49:35 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 00:03:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 00:03:33 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 00:03:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 00:03:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 00:03:36 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:50:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:50:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:50:27 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:50:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:50:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:50:30 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487bef959ea51d4b707107d10bc8bb2cabb35c3d0e890400da9558498fcfae9`  
		Last Modified: Thu, 14 Apr 2022 00:10:34 GMT  
		Size: 112.0 MB (111960610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d226d7216d6a78d6f22f1281ea887106f683641e6690999b23c156756d175`  
		Last Modified: Thu, 14 Apr 2022 00:09:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7dcd4972b24cf7ffe78c888061ef282e320f7a4c8aaa1384a55e7e28bd933c`  
		Last Modified: Thu, 14 Apr 2022 18:52:06 GMT  
		Size: 6.7 MB (6679287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d018e3dc9cc16296861b01cbe8f4be57f1b151d8cb8fa4071917b9226c48f10`  
		Last Modified: Thu, 14 Apr 2022 18:52:03 GMT  
		Size: 1.2 MB (1178511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1905214dc55b0a74bee4af520fc034a0b9d4c7dfdd3066b86dff3fdce85c5531`  
		Last Modified: Thu, 14 Apr 2022 18:52:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:64f5ca12c8d834430cfb57aa19efbe9b392b9adf0d1fd74b7935f608fc02ce2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121556014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a179d43265c854bb5a83f1493e85dbcfdb210e3de82f0b18059e2cdd3b48d8bc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:16:49 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 03:23:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 03:23:16 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 03:23:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 03:23:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 03:23:18 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:56:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:56:20 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:56:21 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:56:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:56:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0a2cd126c67e6f9de5c0d2b9a8677d1f9ddf783df14e2ee2b65a4b837f781f`  
		Last Modified: Thu, 14 Apr 2022 03:32:44 GMT  
		Size: 111.7 MB (111729644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862413253fa7da1bfa2e411396d8013220cad00d664feea8f1757d91782065a3`  
		Last Modified: Thu, 14 Apr 2022 03:31:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edfefe81ed126a91f93489eb7294d5726270035f8a8af38291865530e667992`  
		Last Modified: Thu, 14 Apr 2022 18:57:58 GMT  
		Size: 6.0 MB (5953508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493540bf70a415bb315316c76dc35c0704dc57f314daba4f3eebcafd9c25785`  
		Last Modified: Thu, 14 Apr 2022 18:57:56 GMT  
		Size: 1.2 MB (1176708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca939ad5fc968cce313ac75a2a4ed597b4a30705675ead781704e45af5a55d`  
		Last Modified: Thu, 14 Apr 2022 18:57:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2d4b2c1ce3953888f3934a59ffd6c807bd30b072a0314981958baca7a019c42d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121491404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7780a7fd77a5082b830bf4d183ff31097003d03d4dd7fe43cef0a7f0cde8aa62`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:41:03 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 23:46:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 23:46:11 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 23:46:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 23:46:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 23:46:14 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:40:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:40:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:40:12 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:40:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:40:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:40:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:40:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59105010ca6c9ed528dc03f6c683c1bc8cd362cabe6df8b6ffe5cb7ea9a5d7a6`  
		Last Modified: Wed, 13 Apr 2022 23:49:58 GMT  
		Size: 110.4 MB (110425230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a657773900190e59f0ba6a0b06f6708be5a593336955df99496b40dd24e06d`  
		Last Modified: Wed, 13 Apr 2022 23:49:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb01e300b70916735527d066ade51d96bf1499fcc73f8e20921d8e6583b2ac7`  
		Last Modified: Thu, 14 Apr 2022 18:41:03 GMT  
		Size: 6.9 MB (6928572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812f635ea90b30e39607bf3021b59197a9ba23ba5d22f7f65ad17cd2346f434f`  
		Last Modified: Thu, 14 Apr 2022 18:41:02 GMT  
		Size: 1.1 MB (1148677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e543305854e722a1ec5fce4d10334f7560cffc2d7b85f4949d1d87f74c4dd91`  
		Last Modified: Thu, 14 Apr 2022 18:41:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:5f894752b5db9ada4bcd9c049676af704e39a7a1c485738b77831fb061db7bad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122107711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd51942da1947cb52d47358a88b02ba4ea96564b709f19b7830cd91fd91ee97e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:42:52 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 00:33:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 00:33:21 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 00:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 00:33:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 00:33:37 GMT
WORKDIR /go
# Thu, 14 Apr 2022 19:18:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 19:18:33 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:18:34 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 19:18:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 19:18:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b7b70e9365a42d1502d1309f3dc8545df5b5eb802bf656ac8d1a9adc0ca38e`  
		Last Modified: Thu, 14 Apr 2022 00:38:51 GMT  
		Size: 110.6 MB (110577271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de52b4fb28789c7d8a190d4b1275b480c68ef6db3f548db9e61dc0bd5f2287c2`  
		Last Modified: Thu, 14 Apr 2022 00:38:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90034960a371e7877490974def61ec2afab2b9037cf021f8b268adf23f745b1f`  
		Last Modified: Thu, 14 Apr 2022 19:19:39 GMT  
		Size: 7.3 MB (7323527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d57f6a3fec72c6a2cf4c2a1eb8ecebd37651cec4da21115e9e32dd8f03bbf7e`  
		Last Modified: Thu, 14 Apr 2022 19:19:37 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05805de310a20ace9a3d0ef07f9421ee52c90b90cc848a5e33739ad6a59922c5`  
		Last Modified: Thu, 14 Apr 2022 19:19:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:bbd242c619b69514e71d5da5eb45237d807ae613391e2c9747270f52353e2b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124494420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d34717a0d196251ad9ecf3ad7c2cde4dba578edce1cd1a5d6f3acf9e9ce44c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:42:49 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 23:53:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 23:54:15 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 23:54:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 23:54:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 23:54:18 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:41:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:41:58 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:41:58 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:41:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:41:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ce7cc2608f8fa7ccebc2bd15f044fe91007681fdf9e3497b835c6671ea698`  
		Last Modified: Thu, 14 Apr 2022 00:01:54 GMT  
		Size: 113.5 MB (113483469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eebd463aa6406b85ba12e73255070fbd1566b013a0ca9f3fb5d3ccf5887df95`  
		Last Modified: Thu, 14 Apr 2022 00:01:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324a2146e85ce6ede318cd28053e0977db3f0488b3ce78af656c65965e9001c`  
		Last Modified: Thu, 14 Apr 2022 18:42:50 GMT  
		Size: 6.9 MB (6933814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e38c01e4bbf4761ba513566ff71938324df91b374aa5ac65af00f459114d6`  
		Last Modified: Thu, 14 Apr 2022 18:42:49 GMT  
		Size: 1.2 MB (1203782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c3ddda25fbe6281766300073c154f69301b0f4de46963a08615b935ae1ea0d`  
		Last Modified: Thu, 14 Apr 2022 18:42:49 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:fe51fdb546253aaa85f6ce127801e69a59ced7d4b63e4129651bdd2c36055947
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888961958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa784331ba2917985c784f282d3e9291e48bce67a5ba731c334475e3e8ed497`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:19:50 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:21:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 14 Apr 2022 19:21:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32cd6fe077128d0ff8716ad4ee3897dcbcdf1c5186746faa4c3bbc9459b5727`  
		Last Modified: Thu, 14 Apr 2022 19:23:08 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699d3aa3b585eb438b00131501e3f2319fd71d3974d72076206bba6294e52252`  
		Last Modified: Thu, 14 Apr 2022 19:23:07 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5244079ba82287cefa9f1afd23b8e818bc55d7228ec81f9d675b764afb021b7e`  
		Last Modified: Thu, 14 Apr 2022 19:23:09 GMT  
		Size: 1.7 MB (1663026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d4ca102f25be2a1c45d0e8ff9a0dedd40a6e5c30fd3d895e6155de8c4fc61d`  
		Last Modified: Thu, 14 Apr 2022 19:23:07 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:4561488a658c02262b4bc7a28527d8d1d4d4d829a0be740d1e82e992c491c85e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2408027806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7a60b7fdfbc4ef924c96c2c9f70f261a6c0150470531fc689c37e7f3053e45`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:27:59 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:28:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:28:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:28:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:29:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:29:19 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:30:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:30:08 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 02:33:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c30bc3f1f7314a953fe208bd9cd5e24bd9403392a6c556ced3677f9f70f71fe1'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:33:49 GMT
WORKDIR C:\go
# Thu, 14 Apr 2022 19:21:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Apr 2022 19:21:18 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:21:19 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:21:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:21:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 14 Apr 2022 19:21:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df2c1d7d7b9748c6ddb8e9f196dfb2526451470a1256ab4047bece8468ff7a`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9395e3155b04f913275d2f0e2bd07626c8d9b889b0646bb3fb44414d2df4130d`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d0b098f175d5015767a5bb9a5641f1a1966ea2e2863b55cae5ae54f7edeb9`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff921731e5c58ad62f0eb62e698dd3033694fd15898c3e94d8021c0097dd912`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b89723742f5296cfb0b6d93c8b65a4995ee4a964d59eae8e96557dffc8f9e`  
		Last Modified: Wed, 13 Apr 2022 03:14:02 GMT  
		Size: 25.7 MB (25714775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab0e7bcbbef7fb8a566a25556fc4b487c323359badbd7ab1bc58ab41729a7a`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f67794576dcaaf4ef811c935b4ed0b40efe1487f0d0ab09462473b606d1fd89`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 562.2 KB (562186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932986f0f385a406d2115ccb58dbf32a1730cf7e1f7f9f520863fcaa3e20d64`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f896ebd03d7af93409bcfb6bbbbd64481e6f575754cf0c600003a48a32d7a0b`  
		Last Modified: Wed, 13 Apr 2022 03:14:42 GMT  
		Size: 152.9 MB (152877366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f82b1974e8addd899731575590ff20cf09b3e97cdfe2ed285fc081b742b331`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52686327c4846c19f28b539d50b9d61e28b6fea5b5fddd0b921f8cbeb53d872e`  
		Last Modified: Thu, 14 Apr 2022 19:23:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40034260ba3cdfd11f2724f7ae8f01f12903d459a60864dcfe43f83d0de04a18`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b648565257aa7a6856b0995547e2df5a44b07dcc09764ff784309e169801b1d0`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362ba6dc5120c248e50d6eca168d2bb19ddedacb17077d216f1ee35a2ea80d18`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0639ab661b6c6742c087940cd20ac05a0641da5a31d2633cf9e775fe0f052b7`  
		Last Modified: Thu, 14 Apr 2022 19:23:18 GMT  
		Size: 1.9 MB (1900229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648f5012dc3efea00a4abafd625cf013c9a8359f484b59bb678d1283f448df5`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-builder-alpine`

```console
$ docker pull caddy@sha256:111c414652d39ff8c17392480a4d1c5ca09b130176ca5cc401ef0753d9e70801
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.0-rc.1-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:39f14f117c0b3b4231d479b39592c96fe51d84503489ca70d2d6213b73b1371f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126725956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5332e4589600d01eb51e2690698aa0b12d8bcaf376e43b54be72b9f6f0ce913`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:20:33 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 02:34:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 02:34:25 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 02:34:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 02:34:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 02:34:25 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:19:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:19:34 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:19:34 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:19:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:19:35 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:19:35 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:19:36 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6858aa20941bdfe0d406b2e4db477feeccf42ca6e40478043b721c6a66f9d1b6`  
		Last Modified: Thu, 14 Apr 2022 02:37:21 GMT  
		Size: 115.6 MB (115569906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8029b02d49777774618d41ab3a1f7f4f32f7d4b10453afd26a184b8787beaa`  
		Last Modified: Thu, 14 Apr 2022 02:37:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8852fa41bd6ab92e973a3316d6db4a27e9b1844abac8363c94c241958de8ad22`  
		Last Modified: Thu, 14 Apr 2022 18:20:07 GMT  
		Size: 6.8 MB (6823100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8824e5886ff61d400983eba90a9e3fd8fff37ed666dc3fbf532fb19336de59f0`  
		Last Modified: Thu, 14 Apr 2022 18:20:06 GMT  
		Size: 1.2 MB (1245713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935ac112e2d54d80c0e13be0791314cff9e6b1bec42d9354f90ff9c6bfedce2a`  
		Last Modified: Thu, 14 Apr 2022 18:20:06 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:638fe015b430dbd80bce39acaac9474eeef1183ca69eccba20942cbe5f7b62ea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122713231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb1ec6719298af0eae4e8c888c1a237942d068f190bda4b72fa419c9e9667080`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:49:35 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 00:03:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 00:03:33 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 00:03:34 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 00:03:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 00:03:36 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:50:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:50:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:50:27 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:50:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:50:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:50:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:50:30 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d487bef959ea51d4b707107d10bc8bb2cabb35c3d0e890400da9558498fcfae9`  
		Last Modified: Thu, 14 Apr 2022 00:10:34 GMT  
		Size: 112.0 MB (111960610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232d226d7216d6a78d6f22f1281ea887106f683641e6690999b23c156756d175`  
		Last Modified: Thu, 14 Apr 2022 00:09:20 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd7dcd4972b24cf7ffe78c888061ef282e320f7a4c8aaa1384a55e7e28bd933c`  
		Last Modified: Thu, 14 Apr 2022 18:52:06 GMT  
		Size: 6.7 MB (6679287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d018e3dc9cc16296861b01cbe8f4be57f1b151d8cb8fa4071917b9226c48f10`  
		Last Modified: Thu, 14 Apr 2022 18:52:03 GMT  
		Size: 1.2 MB (1178511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1905214dc55b0a74bee4af520fc034a0b9d4c7dfdd3066b86dff3fdce85c5531`  
		Last Modified: Thu, 14 Apr 2022 18:52:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:64f5ca12c8d834430cfb57aa19efbe9b392b9adf0d1fd74b7935f608fc02ce2a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121556014 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a179d43265c854bb5a83f1493e85dbcfdb210e3de82f0b18059e2cdd3b48d8bc`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:16:49 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 03:23:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 03:23:16 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 03:23:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 03:23:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 03:23:18 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:56:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:56:20 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:56:21 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:56:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:56:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:56:23 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:56:24 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0a2cd126c67e6f9de5c0d2b9a8677d1f9ddf783df14e2ee2b65a4b837f781f`  
		Last Modified: Thu, 14 Apr 2022 03:32:44 GMT  
		Size: 111.7 MB (111729644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:862413253fa7da1bfa2e411396d8013220cad00d664feea8f1757d91782065a3`  
		Last Modified: Thu, 14 Apr 2022 03:31:31 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edfefe81ed126a91f93489eb7294d5726270035f8a8af38291865530e667992`  
		Last Modified: Thu, 14 Apr 2022 18:57:58 GMT  
		Size: 6.0 MB (5953508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b493540bf70a415bb315316c76dc35c0704dc57f314daba4f3eebcafd9c25785`  
		Last Modified: Thu, 14 Apr 2022 18:57:56 GMT  
		Size: 1.2 MB (1176708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ca939ad5fc968cce313ac75a2a4ed597b4a30705675ead781704e45af5a55d`  
		Last Modified: Thu, 14 Apr 2022 18:57:55 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:2d4b2c1ce3953888f3934a59ffd6c807bd30b072a0314981958baca7a019c42d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121491404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7780a7fd77a5082b830bf4d183ff31097003d03d4dd7fe43cef0a7f0cde8aa62`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:41:03 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 23:46:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 23:46:11 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 23:46:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 23:46:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 23:46:14 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:40:10 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:40:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:40:12 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:40:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:40:15 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:40:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:40:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59105010ca6c9ed528dc03f6c683c1bc8cd362cabe6df8b6ffe5cb7ea9a5d7a6`  
		Last Modified: Wed, 13 Apr 2022 23:49:58 GMT  
		Size: 110.4 MB (110425230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a657773900190e59f0ba6a0b06f6708be5a593336955df99496b40dd24e06d`  
		Last Modified: Wed, 13 Apr 2022 23:49:43 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb01e300b70916735527d066ade51d96bf1499fcc73f8e20921d8e6583b2ac7`  
		Last Modified: Thu, 14 Apr 2022 18:41:03 GMT  
		Size: 6.9 MB (6928572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812f635ea90b30e39607bf3021b59197a9ba23ba5d22f7f65ad17cd2346f434f`  
		Last Modified: Thu, 14 Apr 2022 18:41:02 GMT  
		Size: 1.1 MB (1148677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e543305854e722a1ec5fce4d10334f7560cffc2d7b85f4949d1d87f74c4dd91`  
		Last Modified: Thu, 14 Apr 2022 18:41:02 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:5f894752b5db9ada4bcd9c049676af704e39a7a1c485738b77831fb061db7bad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122107711 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd51942da1947cb52d47358a88b02ba4ea96564b709f19b7830cd91fd91ee97e`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:42:52 GMT
ENV GOLANG_VERSION=1.18.1
# Thu, 14 Apr 2022 00:33:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 14 Apr 2022 00:33:21 GMT
ENV GOPATH=/go
# Thu, 14 Apr 2022 00:33:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 14 Apr 2022 00:33:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 14 Apr 2022 00:33:37 GMT
WORKDIR /go
# Thu, 14 Apr 2022 19:18:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 19:18:33 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:18:34 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 19:18:46 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 19:18:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b7b70e9365a42d1502d1309f3dc8545df5b5eb802bf656ac8d1a9adc0ca38e`  
		Last Modified: Thu, 14 Apr 2022 00:38:51 GMT  
		Size: 110.6 MB (110577271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de52b4fb28789c7d8a190d4b1275b480c68ef6db3f548db9e61dc0bd5f2287c2`  
		Last Modified: Thu, 14 Apr 2022 00:38:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90034960a371e7877490974def61ec2afab2b9037cf021f8b268adf23f745b1f`  
		Last Modified: Thu, 14 Apr 2022 19:19:39 GMT  
		Size: 7.3 MB (7323527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d57f6a3fec72c6a2cf4c2a1eb8ecebd37651cec4da21115e9e32dd8f03bbf7e`  
		Last Modified: Thu, 14 Apr 2022 19:19:37 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05805de310a20ace9a3d0ef07f9421ee52c90b90cc848a5e33739ad6a59922c5`  
		Last Modified: Thu, 14 Apr 2022 19:19:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bbd242c619b69514e71d5da5eb45237d807ae613391e2c9747270f52353e2b78
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124494420 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3d34717a0d196251ad9ecf3ad7c2cde4dba578edce1cd1a5d6f3acf9e9ce44c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:42:49 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 23:53:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.1.src.tar.gz'; 		sha256='efd43e0f1402e083b73a03d444b7b6576bb4c539ac46208b63a916b69aca4088'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 23:54:15 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 23:54:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 23:54:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 23:54:18 GMT
WORKDIR /go
# Thu, 14 Apr 2022 18:41:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 14 Apr 2022 18:41:58 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 18:41:58 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 18:41:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 18:41:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 14 Apr 2022 18:41:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 14 Apr 2022 18:41:59 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265ce7cc2608f8fa7ccebc2bd15f044fe91007681fdf9e3497b835c6671ea698`  
		Last Modified: Thu, 14 Apr 2022 00:01:54 GMT  
		Size: 113.5 MB (113483469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eebd463aa6406b85ba12e73255070fbd1566b013a0ca9f3fb5d3ccf5887df95`  
		Last Modified: Thu, 14 Apr 2022 00:01:38 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7324a2146e85ce6ede318cd28053e0977db3f0488b3ce78af656c65965e9001c`  
		Last Modified: Thu, 14 Apr 2022 18:42:50 GMT  
		Size: 6.9 MB (6933814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1e38c01e4bbf4761ba513566ff71938324df91b374aa5ac65af00f459114d6`  
		Last Modified: Thu, 14 Apr 2022 18:42:49 GMT  
		Size: 1.2 MB (1203782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7c3ddda25fbe6281766300073c154f69301b0f4de46963a08615b935ae1ea0d`  
		Last Modified: Thu, 14 Apr 2022 18:42:49 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:1b1855eacf28accf736b7c86dbefd11acd0f1c60658e60e42edee399bf297503
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.5.0-rc.1-builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:fe51fdb546253aaa85f6ce127801e69a59ced7d4b63e4129651bdd2c36055947
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888961958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:baa784331ba2917985c784f282d3e9291e48bce67a5ba731c334475e3e8ed497`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:19:50 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:19:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:21:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 14 Apr 2022 19:21:01 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32cd6fe077128d0ff8716ad4ee3897dcbcdf1c5186746faa4c3bbc9459b5727`  
		Last Modified: Thu, 14 Apr 2022 19:23:08 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699d3aa3b585eb438b00131501e3f2319fd71d3974d72076206bba6294e52252`  
		Last Modified: Thu, 14 Apr 2022 19:23:07 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5244079ba82287cefa9f1afd23b8e818bc55d7228ec81f9d675b764afb021b7e`  
		Last Modified: Thu, 14 Apr 2022 19:23:09 GMT  
		Size: 1.7 MB (1663026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d4ca102f25be2a1c45d0e8ff9a0dedd40a6e5c30fd3d895e6155de8c4fc61d`  
		Last Modified: Thu, 14 Apr 2022 19:23:07 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:903cb3434c2aadd79a07111e9bc2540f01c83529f26d829e2233062bcd88c3fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-rc.1-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:4561488a658c02262b4bc7a28527d8d1d4d4d829a0be740d1e82e992c491c85e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2408027806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7a60b7fdfbc4ef924c96c2c9f70f261a6c0150470531fc689c37e7f3053e45`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:27:59 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:28:00 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:28:01 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:28:02 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:29:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:29:19 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:30:07 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:30:08 GMT
ENV GOLANG_VERSION=1.18.1
# Wed, 13 Apr 2022 02:33:47 GMT
RUN $url = 'https://dl.google.com/go/go1.18.1.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'c30bc3f1f7314a953fe208bd9cd5e24bd9403392a6c556ced3677f9f70f71fe1'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:33:49 GMT
WORKDIR C:\go
# Thu, 14 Apr 2022 19:21:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Apr 2022 19:21:18 GMT
ENV XCADDY_VERSION=v0.2.1
# Thu, 14 Apr 2022 19:21:19 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:21:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 14 Apr 2022 19:21:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 14 Apr 2022 19:21:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46df2c1d7d7b9748c6ddb8e9f196dfb2526451470a1256ab4047bece8468ff7a`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9395e3155b04f913275d2f0e2bd07626c8d9b889b0646bb3fb44414d2df4130d`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d0b098f175d5015767a5bb9a5641f1a1966ea2e2863b55cae5ae54f7edeb9`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff921731e5c58ad62f0eb62e698dd3033694fd15898c3e94d8021c0097dd912`  
		Last Modified: Wed, 13 Apr 2022 03:13:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19b89723742f5296cfb0b6d93c8b65a4995ee4a964d59eae8e96557dffc8f9e`  
		Last Modified: Wed, 13 Apr 2022 03:14:02 GMT  
		Size: 25.7 MB (25714775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ab0e7bcbbef7fb8a566a25556fc4b487c323359badbd7ab1bc58ab41729a7a`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f67794576dcaaf4ef811c935b4ed0b40efe1487f0d0ab09462473b606d1fd89`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 562.2 KB (562186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2932986f0f385a406d2115ccb58dbf32a1730cf7e1f7f9f520863fcaa3e20d64`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f896ebd03d7af93409bcfb6bbbbd64481e6f575754cf0c600003a48a32d7a0b`  
		Last Modified: Wed, 13 Apr 2022 03:14:42 GMT  
		Size: 152.9 MB (152877366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f82b1974e8addd899731575590ff20cf09b3e97cdfe2ed285fc081b742b331`  
		Last Modified: Wed, 13 Apr 2022 03:13:40 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52686327c4846c19f28b539d50b9d61e28b6fea5b5fddd0b921f8cbeb53d872e`  
		Last Modified: Thu, 14 Apr 2022 19:23:18 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40034260ba3cdfd11f2724f7ae8f01f12903d459a60864dcfe43f83d0de04a18`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b648565257aa7a6856b0995547e2df5a44b07dcc09764ff784309e169801b1d0`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362ba6dc5120c248e50d6eca168d2bb19ddedacb17077d216f1ee35a2ea80d18`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0639ab661b6c6742c087940cd20ac05a0641da5a31d2633cf9e775fe0f052b7`  
		Last Modified: Thu, 14 Apr 2022 19:23:18 GMT  
		Size: 1.9 MB (1900229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8648f5012dc3efea00a4abafd625cf013c9a8359f484b59bb678d1283f448df5`  
		Last Modified: Thu, 14 Apr 2022 19:23:16 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-windowsservercore`

```console
$ docker pull caddy@sha256:521bb74789f77e498ee1d3ec122928e4e667f936f61d680d73feb727a648e1df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2803; amd64
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-rc.1-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:7b19b5e3e5e35dde6a6cccda23e08c5c85cf68721e7bef80738dd82d935b1b16
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2730640494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ffd5b6e5907cb60d7a5adb0c56dc9053176223ecbf2bf5fcff3399f5f49e0f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:14:49 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:16:18 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:16:19 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:16:20 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:16:21 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:16:22 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:16:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:16:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:16:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:16:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:16:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:16:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:16:29 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:16:30 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:16:31 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:17:24 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12da94364e01a36d779bfafc8863ca1f7bf8234ce6f24988f68d1fd00ee02e06`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8ad753593036d1913b13edebd4355a905b469d0a9620d971dc9715f86e8ea2`  
		Last Modified: Thu, 14 Apr 2022 19:22:43 GMT  
		Size: 14.0 MB (13996925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c46084e73c5bf425af70578d2b0c76fabdccb126bc44c08c416817c1b6afe9c`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15af6c7018758c35ce48abb844810310bc64a68a6652695fc2de9b22707776b`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a6e7263b523e92d854d0cc0b89aadce4caeacc6525564cec3c2571bd621cd`  
		Last Modified: Thu, 14 Apr 2022 19:22:38 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04936128e7337a3425482423730fa939d21156c82597e0a3590049ed0a2fde57`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29420237ea837193935f4775de4cde39f9f998736b5298de43e472020d1d71df`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c94746d51b500baa19679f8aea92c90c46f6cac1d3040961911118da7432c1`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e02a7405a7e431869559ca1835268f104d17cc01aef969b01ce7929db2a5a5`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8372ff9d2fac7726f43c23f9c7f476ffd605f83ba9620d249300acf8607c2db`  
		Last Modified: Thu, 14 Apr 2022 19:22:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8b5f63b11c418280546ef6ed46310b89e4278ba33166610d216c24972be24`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a09cab4711bf91a1a3a3748a4c71bd78e41e199e554cc9a7c4173bcbe5c8515`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ce147cef3583f85a61794253d22dda5c99730a5b9362f69f2b40fe5baf7d34`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08658cd1da7ac20abe49b3609c5409267fcf83f9f14d854b6b72507b466ce003`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbdbe95ffca8c3113ef88ec04d897761f94fe44c70bc1d7bec368990ad24a6`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb5a4353c7ad939cf38f5f9e00cc9bd752ad926af8c9616942abdc79c3363`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4100dac27cedd92e1030d8b5a435307675c7c8f43b30b3b7a5d7a39ca8ff0f3c`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afafdaac1485785c781de040ff6901dde99b21ed257731f05118bab0c5955cc8`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 319.6 KB (319620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f2db279cae21b2def39302565eeb754e2903fae000c7dcf515d116a6c95aea`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-rc.1-windowsservercore` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:eb507596ef94e6ed3084201996e9f08e25b8745151ee6bedb7d36948dac054c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2242203268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffb97fd117fc020226f103385f120ef0e4e196a279809be3d26b3312a1f76bb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:45:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:17:36 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:18:44 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:18:45 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:18:46 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:18:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:18:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:18:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:18:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:18:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:18:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:18:54 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:18:55 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:18:56 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:19:30 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:19:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ff8ee97053f0fd2c04d1416858c55ed3909995cfc0831aa8f5a40204afd05`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 638.3 KB (638318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357652fda2b1e4d70c62d8d4ba35b476e36dd760b13a3eeacb8226bb50f448a`  
		Last Modified: Thu, 14 Apr 2022 19:22:57 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d217fa02930e4a656c7c4400fd7bb8baf3fa5702845f7e001de598bb9897c1`  
		Last Modified: Thu, 14 Apr 2022 19:23:00 GMT  
		Size: 14.2 MB (14225960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be5ff6bcf52b91e81fc414154427fb0320f1abcfe6cd53291f7b76a3f19cedb`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2215b48dac38251ea50b99034b6ccdbe83b2b4ab6a5e8476ae420eb6ea1507d6`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb351741bf0e672fb7c17e72bec00805d65311f8735a27cd33c428fd8c7db75`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ca0a8ec5cf1007e5e10a1d84ad67ed62967011eeaa10651e4df6599894d25`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978b105b9f03fa4b576a81dcef90374cb71c060548775a02686c100f1f9760e`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4840ed0bb6147c09215fa024ceb9fb9ec6638b7e05f03fde0c65345bc01257`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67111082235827f0f88e06d275ae8b7e1921e9d97e1cbe06b823ee7ad5670aff`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f9d794f6ff120d428bdc2cc5dcaa92736efe0cf104fbf7895e0a9bc4d0fac8`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175c2dc51ad06867c5059b438053a3806f5ef00aca3b9571c5b97db4aaecdf4`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623f3d22cd9cbdce94520c24cfac311df3e812b677cb5f16987daf5c00b923b`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f4acb76ece48c3ce666ca49abc7a0272959e573fad0222118435a37500fe0`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15acc8553457ab93836f3baa7faca6c62d13191114808e6c88d1c0dcd260307`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f336f0884a81040c8d84becf06b03a72aa1c1db7d627776ebc31681d037a08`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06694bc95a3b5673379a452023fab263afce2e02f3f735b3536478cb542f27e3`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38101d9aa2a7c4427ddc00488619fefd9ee139d7a3523644372beb8e5e95f7`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e25c0f33c7d9786bd26a0bf0d32451d9752eccab24b5cc2089a624c72efeff`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 358.7 KB (358693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ecdd10190bfd15bfb6eda278d94f8f29aadab7210e25a8ea1dbce0a60bd62`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6b423133fb3a07e11c9ba80e23d4ee2abb6bc1b11b4f2bfa208d053f3974d23b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.5.0-rc.1-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:7b19b5e3e5e35dde6a6cccda23e08c5c85cf68721e7bef80738dd82d935b1b16
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2730640494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16ffd5b6e5907cb60d7a5adb0c56dc9053176223ecbf2bf5fcff3399f5f49e0f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:14:49 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:17 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:16:18 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:16:19 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:16:20 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:16:21 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:16:22 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:16:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:16:24 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:16:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:16:26 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:16:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:16:28 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:16:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:16:29 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:16:30 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:16:31 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:17:24 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:17:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12da94364e01a36d779bfafc8863ca1f7bf8234ce6f24988f68d1fd00ee02e06`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8ad753593036d1913b13edebd4355a905b469d0a9620d971dc9715f86e8ea2`  
		Last Modified: Thu, 14 Apr 2022 19:22:43 GMT  
		Size: 14.0 MB (13996925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c46084e73c5bf425af70578d2b0c76fabdccb126bc44c08c416817c1b6afe9c`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15af6c7018758c35ce48abb844810310bc64a68a6652695fc2de9b22707776b`  
		Last Modified: Thu, 14 Apr 2022 19:22:39 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a61a6e7263b523e92d854d0cc0b89aadce4caeacc6525564cec3c2571bd621cd`  
		Last Modified: Thu, 14 Apr 2022 19:22:38 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04936128e7337a3425482423730fa939d21156c82597e0a3590049ed0a2fde57`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29420237ea837193935f4775de4cde39f9f998736b5298de43e472020d1d71df`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03c94746d51b500baa19679f8aea92c90c46f6cac1d3040961911118da7432c1`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7e02a7405a7e431869559ca1835268f104d17cc01aef969b01ce7929db2a5a5`  
		Last Modified: Thu, 14 Apr 2022 19:22:37 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8372ff9d2fac7726f43c23f9c7f476ffd605f83ba9620d249300acf8607c2db`  
		Last Modified: Thu, 14 Apr 2022 19:22:36 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2f8b5f63b11c418280546ef6ed46310b89e4278ba33166610d216c24972be24`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a09cab4711bf91a1a3a3748a4c71bd78e41e199e554cc9a7c4173bcbe5c8515`  
		Last Modified: Thu, 14 Apr 2022 19:22:35 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ce147cef3583f85a61794253d22dda5c99730a5b9362f69f2b40fe5baf7d34`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08658cd1da7ac20abe49b3609c5409267fcf83f9f14d854b6b72507b466ce003`  
		Last Modified: Thu, 14 Apr 2022 19:22:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecbdbe95ffca8c3113ef88ec04d897761f94fe44c70bc1d7bec368990ad24a6`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfeb5a4353c7ad939cf38f5f9e00cc9bd752ad926af8c9616942abdc79c3363`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4100dac27cedd92e1030d8b5a435307675c7c8f43b30b3b7a5d7a39ca8ff0f3c`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afafdaac1485785c781de040ff6901dde99b21ed257731f05118bab0c5955cc8`  
		Last Modified: Thu, 14 Apr 2022 19:22:33 GMT  
		Size: 319.6 KB (319620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f2db279cae21b2def39302565eeb754e2903fae000c7dcf515d116a6c95aea`  
		Last Modified: Thu, 14 Apr 2022 19:22:32 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-rc.1-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:d30f0c6ace4046bc19e229a52c9c41d509758a6b48bf58845da0ea5838f3eabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-rc.1-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:eb507596ef94e6ed3084201996e9f08e25b8745151ee6bedb7d36948dac054c1
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2242203268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dffb97fd117fc020226f103385f120ef0e4e196a279809be3d26b3312a1f76bb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:45:42 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 14 Apr 2022 19:17:36 GMT
ENV CADDY_VERSION=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:41 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-rc.1/caddy_2.5.0-rc.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('3d7b6a2e4384e6dc9c176036c03eecb2f28488e45e85a2db2c6f72eb3bbeb33c29a5830b96d803805223624d8d706ef2c9b4c1c33001b81fae5b159222e7f637')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 14 Apr 2022 19:18:42 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 14 Apr 2022 19:18:44 GMT
VOLUME [c:/config]
# Thu, 14 Apr 2022 19:18:45 GMT
VOLUME [c:/data]
# Thu, 14 Apr 2022 19:18:46 GMT
LABEL org.opencontainers.image.version=v2.5.0-rc.1
# Thu, 14 Apr 2022 19:18:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 14 Apr 2022 19:18:48 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 14 Apr 2022 19:18:49 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 14 Apr 2022 19:18:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 14 Apr 2022 19:18:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 14 Apr 2022 19:18:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 14 Apr 2022 19:18:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 14 Apr 2022 19:18:54 GMT
EXPOSE 80
# Thu, 14 Apr 2022 19:18:55 GMT
EXPOSE 443
# Thu, 14 Apr 2022 19:18:56 GMT
EXPOSE 2019
# Thu, 14 Apr 2022 19:19:30 GMT
RUN caddy version
# Thu, 14 Apr 2022 19:19:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105ff8ee97053f0fd2c04d1416858c55ed3909995cfc0831aa8f5a40204afd05`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 638.3 KB (638318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2357652fda2b1e4d70c62d8d4ba35b476e36dd760b13a3eeacb8226bb50f448a`  
		Last Modified: Thu, 14 Apr 2022 19:22:57 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d217fa02930e4a656c7c4400fd7bb8baf3fa5702845f7e001de598bb9897c1`  
		Last Modified: Thu, 14 Apr 2022 19:23:00 GMT  
		Size: 14.2 MB (14225960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be5ff6bcf52b91e81fc414154427fb0320f1abcfe6cd53291f7b76a3f19cedb`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2215b48dac38251ea50b99034b6ccdbe83b2b4ab6a5e8476ae420eb6ea1507d6`  
		Last Modified: Thu, 14 Apr 2022 19:22:56 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb351741bf0e672fb7c17e72bec00805d65311f8735a27cd33c428fd8c7db75`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:068ca0a8ec5cf1007e5e10a1d84ad67ed62967011eeaa10651e4df6599894d25`  
		Last Modified: Thu, 14 Apr 2022 19:22:55 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5978b105b9f03fa4b576a81dcef90374cb71c060548775a02686c100f1f9760e`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4840ed0bb6147c09215fa024ceb9fb9ec6638b7e05f03fde0c65345bc01257`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67111082235827f0f88e06d275ae8b7e1921e9d97e1cbe06b823ee7ad5670aff`  
		Last Modified: Thu, 14 Apr 2022 19:22:54 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f9d794f6ff120d428bdc2cc5dcaa92736efe0cf104fbf7895e0a9bc4d0fac8`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5175c2dc51ad06867c5059b438053a3806f5ef00aca3b9571c5b97db4aaecdf4`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e623f3d22cd9cbdce94520c24cfac311df3e812b677cb5f16987daf5c00b923b`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962f4acb76ece48c3ce666ca49abc7a0272959e573fad0222118435a37500fe0`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15acc8553457ab93836f3baa7faca6c62d13191114808e6c88d1c0dcd260307`  
		Last Modified: Thu, 14 Apr 2022 19:22:52 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f336f0884a81040c8d84becf06b03a72aa1c1db7d627776ebc31681d037a08`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06694bc95a3b5673379a452023fab263afce2e02f3f735b3536478cb542f27e3`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b38101d9aa2a7c4427ddc00488619fefd9ee139d7a3523644372beb8e5e95f7`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e25c0f33c7d9786bd26a0bf0d32451d9752eccab24b5cc2089a624c72efeff`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 358.7 KB (358693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf5ecdd10190bfd15bfb6eda278d94f8f29aadab7210e25a8ea1dbce0a60bd62`  
		Last Modified: Thu, 14 Apr 2022 19:22:50 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:15e576e7d00b1f41a648c5295a03677c24da5fede09131edcb1e6d809c7dc8aa
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
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:c41bdf72cba4e0b7dea13a24c6a77d208ad4c56ba26ae6315e8b7298ee2911de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:b40a94d059874b25babe8cc3bf242e235761309e1454e9db7f36a0dd72bfa6b5
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
$ docker pull caddy@sha256:2f9052dbaf54dfc5934c1c0f9e2d53acaffe0f9e64b47f6ba2c8b95ad2bc9b80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4fb1ee8fe4d7702096d54e6a71c30dbb57b04c59099b5a32e21d127178b56fe`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 05:32:39 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 05:32:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 05:32:40 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:24:42 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:26:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:26:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:26:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:26:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:26:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 02:49:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 02:49:12 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 02:49:13 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 02:49:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52dc419b0ee22d1bb5f3b95a57b2edc733b7b585277f8101db7b2c9b53605c1b`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 272.0 KB (271965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25bc292e5bacdd8b97a1632a82d0fd0ee6c2692409bd4b35cb9e7e652efbc7c8`  
		Last Modified: Tue, 05 Apr 2022 05:42:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:447a8d7240ef06b915ded3f3837852c172f438c860eca533a9cda1442d258c13`  
		Last Modified: Wed, 13 Apr 2022 02:33:15 GMT  
		Size: 110.2 MB (110240209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1849c0ca460162eccf24ec388b1da86b0a755ecf24754307ec19cf6db259931`  
		Last Modified: Wed, 13 Apr 2022 02:33:00 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8a661b382418dc847b4f9817bda67edf55e14cbd3dda8781a1ea813fa67bcbb`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 6.8 MB (6823074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8511c7b8553c34f330183d49b0998b08377c8f143a1e2a5e241fbc41f048067a`  
		Last Modified: Wed, 13 Apr 2022 02:49:41 GMT  
		Size: 1.2 MB (1245714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b691777b7f593a053cc32fcc647ce810bf8d4f7b96e40f55c29609a6f7e10db`  
		Last Modified: Wed, 13 Apr 2022 02:49:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:7d6b4e860ea4e36e832e1c7099ace951337a32cac9dacd61010a3256e8f70ba8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dbb63d72703fbdc83d4a195dfcc9080b44d7e773714f6ab89381d5b761ae55`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 11:39:45 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 11:59:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 11:59:34 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:57:53 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:01:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 03:01:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 03:01:19 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 03:01:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 03:01:21 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:28:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:28:40 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:28:41 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:28:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:28:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:28:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:28:45 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560305eea4784da98378676b22f9871093d6a4d7eb88292accc17f0cfd6b12ea`  
		Last Modified: Tue, 05 Apr 2022 11:40:22 GMT  
		Size: 272.1 KB (272138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a805e932abbcca6b77ad458c7ac26275ff4f23af9912d2c4d3dac9eef4cf8`  
		Last Modified: Tue, 05 Apr 2022 12:15:57 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64a63de7f9cb80c9c8dc52a588b3cb026ac9b81b9f9f4eee061f26f7ac92f53`  
		Last Modified: Wed, 13 Apr 2022 03:11:07 GMT  
		Size: 105.1 MB (105074752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3ef9ff258a9b22dc72b3e3347faaa7d6ccee0a0a349409cd90f807ab3301d3`  
		Last Modified: Wed, 13 Apr 2022 03:09:57 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa22212287529c685f1ee78feb7c126319d73c3f40c0d2e671250557983a1686`  
		Last Modified: Wed, 13 Apr 2022 03:30:30 GMT  
		Size: 6.7 MB (6679294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd66721869fe8d00dd8814d84220f354e26cf909abb6f305cc1f87d8acb7e3e`  
		Last Modified: Wed, 13 Apr 2022 03:30:28 GMT  
		Size: 1.2 MB (1178513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d74b78efbaf46b7ecd95bd09c56b482f10551f3a85e2c56b799b82bbdc8eda`  
		Last Modified: Wed, 13 Apr 2022 03:30:27 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fa8995adb855e7abb6d2edd60b495f81add32e04f9a39fcbe6efa2bc43184337
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114694291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a61afe4da0233acaf545132193d70123741bb3db99f325ca4059dcbf8aec11`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:19:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:19:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:19:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:27:06 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 04:30:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 04:30:18 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 04:30:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 04:30:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 04:30:20 GMT
WORKDIR /go
# Wed, 13 Apr 2022 05:20:30 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 05:20:31 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 05:20:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 05:20:34 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 05:20:34 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 05:20:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63f68dacdb1dfe1ed299ab3e43e478a27f0977380bbefc4c7ca5723758dbac6`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 271.1 KB (271116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5431ad618c287090e481554b57afdc0383f065b5bbfc0ccdcefc6518e1a8331e`  
		Last Modified: Tue, 05 Apr 2022 09:38:23 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbc6f5289dc6298f923d6fc12017734d9e8586e24b541356ac698635ff4b3bf`  
		Last Modified: Wed, 13 Apr 2022 04:50:10 GMT  
		Size: 104.9 MB (104867917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5ef51fb36e825237bfe179dd8b9f19f1be45d8013c3c7b6629e28c02d9cb1e`  
		Last Modified: Wed, 13 Apr 2022 04:48:59 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12de93235cb1b76e396db24c566bf2a468069e2d950bdc72f50e83107b607b89`  
		Last Modified: Wed, 13 Apr 2022 05:22:21 GMT  
		Size: 6.0 MB (5953507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ffdac0197d349fd8bf23bb4abb63de164784fae8f2610656a90c4dd2313395`  
		Last Modified: Wed, 13 Apr 2022 05:22:20 GMT  
		Size: 1.2 MB (1176712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25c50dffdf0d59dcdab4491e71e6873cc5b87b8045f90059ae86d3de4af29bd3`  
		Last Modified: Wed, 13 Apr 2022 05:22:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a007bcff0f7a2db75fd0fec8d444a59164a6eb413c359b36286cb74862620b27
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6e59868b3746a3f33005cc3e6fe76a3cd0ccb8046ae928ff86e97feb7f8317`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:38:07 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 07:38:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:38:08 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:45:36 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:46:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:46:55 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:46:56 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:46:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:46:58 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:10:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:10:21 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:10:21 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:10:22 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:26 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7637d0a7b497b253b73e807a5e676ba3f0750afafa9e1a4c61260513feb321f`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 271.8 KB (271764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda57b85efde0ed435315f4f74625e7a055107aa29e8c91a313ca6d525fb709c`  
		Last Modified: Tue, 05 Apr 2022 07:45:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b49713a5d3bb0c356fa9c8fc70b5dafa275f19861e12ee2287a1b1ab50d06911`  
		Last Modified: Wed, 13 Apr 2022 02:54:09 GMT  
		Size: 104.5 MB (104472805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8fb42bb649cca1e4a9427e17aefb723d3ffd4ec35381839c591618eb2dacb4f`  
		Last Modified: Wed, 13 Apr 2022 02:53:54 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b43ea3c71b0c94063ae30e70a7be5332c37845fcc328caa81a469f589bbc438`  
		Last Modified: Wed, 13 Apr 2022 03:11:19 GMT  
		Size: 6.9 MB (6928494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b7e830aa6764addb02e254edd55f979ae6c48b5f5da144d39155cc6a0f597`  
		Last Modified: Wed, 13 Apr 2022 03:11:18 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897d051b90d84a44772b416bc9b0703767642de938eb0365be3deee57aa0d96e`  
		Last Modified: Wed, 13 Apr 2022 03:11:17 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f2b9d27e0e3b74d7c88c2d7c6497de86655ebfea976efb1419094e1640ab342a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb3c788887767e06270b8307d258aa1ef43bc64968fe1aa06f3be827df8bce42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:50:13 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 09:50:19 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 09:50:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:09 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:51:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:51:08 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:51:10 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:51:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:51:22 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:15:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:15:26 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:15:29 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:15:31 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:15:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:15:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:15:46 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcdc2e904e95f788aa4c66c5ce746890d6a02abca4c94711443f5c688b61ebf`  
		Last Modified: Tue, 05 Apr 2022 10:06:11 GMT  
		Size: 274.2 KB (274171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04802687d9aa11413122df45eb15c7d7f85937270997b441d1c6a09001730453`  
		Last Modified: Tue, 05 Apr 2022 10:06:10 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462fed2c8c2b7766de21b3fa061a4bdf5e36a2dd772ba02edef52d8f32189d6a`  
		Last Modified: Wed, 13 Apr 2022 02:58:43 GMT  
		Size: 102.8 MB (102844156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5723cd64cbc719f56282d94fba9119a33a3d3284aee4f9abd462b8b1788c74`  
		Last Modified: Wed, 13 Apr 2022 02:58:25 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:830351ffaa7e74accb22fa6c61e7461595f2e138f81f74a42a8aeb964fcebfc2`  
		Last Modified: Wed, 13 Apr 2022 03:17:09 GMT  
		Size: 7.3 MB (7323524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536ad6920bf7c84c4dbecb6ec1ad116c33f66836ff3603472f328b7d875671b1`  
		Last Modified: Wed, 13 Apr 2022 03:17:08 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bea1aeeefdc619b79ff52c818c9d3103631b40d7f426a82140d63d7c2a99bc84`  
		Last Modified: Wed, 13 Apr 2022 03:17:07 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:cf9076234739bf3fc87868b34d90ad2d8538a69a63c23b07b37e57abac03cb28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdf45dcc8a69bfd37d14851bde38e4982e415e3df7e2e7a84d811c94d2bfb67f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:08:51 GMT
RUN apk add --no-cache ca-certificates
# Tue, 05 Apr 2022 06:44:34 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:44:35 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:48:28 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.9.src.tar.gz'; 		sha256='763ad4bafb80a9204458c5fa2b8e7327fa971aee454252c0e362c11236156813'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 13 Apr 2022 02:50:06 GMT
ENV GOPATH=/go
# Wed, 13 Apr 2022 02:50:06 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 13 Apr 2022 02:50:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 13 Apr 2022 02:50:07 GMT
WORKDIR /go
# Wed, 13 Apr 2022 03:12:50 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 13 Apr 2022 03:12:50 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 03:12:51 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 03:12:51 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:12:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:12:53 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:12:53 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72593bb761a2ce336603e9e84973d1e284f39e0188e758ad8bc22c45cd9b6395`  
		Last Modified: Tue, 05 Apr 2022 06:09:13 GMT  
		Size: 272.3 KB (272267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf480933488ffcb2c9c9269292e2e3d643bea6eeb04cf948790ca50666a61c8`  
		Last Modified: Tue, 05 Apr 2022 06:53:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd693e9004e149376682b220bdfbad9148604d822d2de750cf7594f02f01f68`  
		Last Modified: Wed, 13 Apr 2022 02:56:37 GMT  
		Size: 107.8 MB (107768303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9dd3fc4ae620c916c57e273173d93db2897c300b815c6c4969ac6c4671b4e2`  
		Last Modified: Wed, 13 Apr 2022 02:56:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff90569da3e4375cca016df4d8757d1c6f9a9a6f3b7d215054b9d5b931280695`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 6.9 MB (6933815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d601ba5248066c3e9604e0e41ebc0b2ba90cf0fb8529b011ed09b5bb0cf921f9`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 1.2 MB (1203790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a341a6d866f386118c6b9ed096fb9b6be320d98aead17ea4289828428b52f21e`  
		Last Modified: Wed, 13 Apr 2022 03:13:50 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:4eed6304aa3dcd2487f2458eb28c35a51333b31ee8a245989fd6a72ab7d0ada6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:4e109ae3674f6c6f89624f5f567f95f999f5b0df6caf154d5c5dfd726f87dbdd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c3d30744a48b86ec57d491e6e151bf73a6f2032aa729c64190d1aef1a4e519e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 02:34:09 GMT
ENV GIT_VERSION=2.23.0
# Wed, 13 Apr 2022 02:34:10 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 13 Apr 2022 02:34:13 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 13 Apr 2022 02:34:22 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 13 Apr 2022 02:37:03 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:37:05 GMT
ENV GOPATH=C:\go
# Wed, 13 Apr 2022 02:38:54 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 02:55:20 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 03:02:03 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 03:02:09 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:41:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:41:11 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:41:12 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:41:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:42:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:42:21 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9b761254212cd472f566f902a9830a91c33e94d06fb02a0192e29fe447bf98`  
		Last Modified: Wed, 13 Apr 2022 03:15:11 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210c142bbabba5cac6b3d06dc265578eafda02e9f54b2b955129652065abba5`  
		Last Modified: Wed, 13 Apr 2022 03:15:05 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24b5fea0cadfc385f0501b3cd52647d69ba5dd030f05bc637848ed7298ed45e`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1490fa326c6ac4254cc7e87bd773641c1a74d6d68ef0ee562e1296aa6e5ba09`  
		Last Modified: Wed, 13 Apr 2022 03:15:04 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb5425f63a29b9eb9b5bbbf135d080f8b1d2415a665b41591175a49f41da70d`  
		Last Modified: Wed, 13 Apr 2022 03:15:23 GMT  
		Size: 25.5 MB (25453409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf5f939642f2aaa6426ec58683c461b2fc27f9b92ed53ceea3d53e5f5b8d18d`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1523ec6181c5a38a1257f1181b0b390b0fa168627daeb103a617f04cf11c9666`  
		Last Modified: Wed, 13 Apr 2022 03:15:01 GMT  
		Size: 328.4 KB (328368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6a29e70c078bf2fc470013ea504caa6d82ef66cd3af18be02f62f0d134dff6`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c73a058a0e83dbc0674b085ab0d0151f94531062126dc4b1f43b0084df40fb62`  
		Last Modified: Wed, 13 Apr 2022 03:21:14 GMT  
		Size: 145.6 MB (145578329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde9b48a173bb3f29a006a2592b0bd8c63b07c7323137db4862e9a98fdde16b0`  
		Last Modified: Wed, 13 Apr 2022 03:20:24 GMT  
		Size: 1.5 KB (1520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49552906c9650efac10c4f00d5c31cebf6f940a05f00b03588df052cff5966c5`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c413ca6d8afb37ed0141a7d70605c26e6e41e5eff4bc87310dfc61a4401c2efb`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b4bcf4a2711e0b5cb2da5cb559b24909aa338f368d3707abf4c6864460db2e`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78562e4c0ea533a4cf051d0b9bc839623424c2f916a5ede43fb15f0716caa9e5`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87e585753aa23f898a3a13160e144661683e6a6e158380f4c959ce67481d1d2c`  
		Last Modified: Wed, 13 Apr 2022 04:50:05 GMT  
		Size: 1.7 MB (1661442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3a64286d73ce8637abf3f1f6f9610e0336567c77c2c3595d2afc4491ebc3ca`  
		Last Modified: Wed, 13 Apr 2022 04:50:02 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:53e1462eb68d51b5b2995be1c5d0c631fa67824f3fe37d692fe73ca714a7236f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.2803; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:c8555e2ca66576a4404c2b5f31d843a5378dea6134acb500502901b563efebcf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.8 MB (14842034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ace180df3e668bd7937be4555305fdb7686c68acf2b5514665e2bac99bd266a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 04:24:48 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 04:24:50 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 04:24:50 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 04:24:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:24:52 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:24:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:24:52 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:24:53 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:24:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:24:54 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:24:54 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:24:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe024ea85c2d7fb47ce4f044038d4227cee2a982bca3e26a0ea4772b8b652f9a`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 291.2 KB (291230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438e4a77a6e9c40c3bf1fb392618ac596307733f97d294edb86383ce8ff7e51d`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6d2ebbfc8548ecc1dbf4c7568459e52549b81522cb450d42ada1bf82513a8d`  
		Last Modified: Tue, 05 Apr 2022 04:25:34 GMT  
		Size: 11.7 MB (11726452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5c5f60dbd2d0286f964c9769a4a3396935a60d0d71ac0e3f8eea5c4c20711fb`  
		Last Modified: Tue, 05 Apr 2022 04:25:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:01ed10f530dfa4af76fa0f13bcdde451a934fbd3a2d77e4cfa72dbc5587ac6f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (14049473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c322930340bb73e0796df576638a0214eda5499c8f9b79e4f9af61aeb4da4d2`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:14:11 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:14:13 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:14:14 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:14:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:14:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:14:20 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:14:21 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:14:21 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:14:22 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:14:22 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:14:26 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:14:27 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:14:27 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:14:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28d650105deec735ac6dce2611f274a6cf2d9f60fc811167dd6d644e281a38f5`  
		Last Modified: Tue, 05 Apr 2022 03:17:39 GMT  
		Size: 291.7 KB (291653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f3d66a6432942b556bf7a077c220319708b7fc75279695b4b05fa25166fbaf`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5d8162ee509e3528dd82e497c4057d40064d43d532acc589b4408c08d2b144`  
		Last Modified: Tue, 05 Apr 2022 03:17:46 GMT  
		Size: 11.1 MB (11125784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0ebc13031265ef07e50f9c7658d00ce8d28c00affdf202b6dd849558f06ad6`  
		Last Modified: Tue, 05 Apr 2022 03:17:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:80bf5252e7e8c04e9ff83dd861f7ee4e81bad7b2b52b5c78a43abf0c95818cf7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13831303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0dddbbfbbc47ddc2ad3b96622c35ee55ec3eecd5e37cde28c3dfe807ac0827ba`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:52 GMT
ADD file:97f7b59ed0e40e7771daab294820763a7bb86c843317be55725baf1cab39aa12 in / 
# Mon, 04 Apr 2022 23:57:52 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:32:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:32:19 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:32:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:32:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:32:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:32:26 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:32:27 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:32:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:32:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:32:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:32:31 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:32:31 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:32:32 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:32:33 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:32:33 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:380010979fdd8a9a4b0bf397034a27ec6cabe61d36e9e6d460ea986f0ddaef38`  
		Last Modified: Mon, 04 Apr 2022 23:59:45 GMT  
		Size: 2.4 MB (2427969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0decd23e3d353b46346bc943e7c39f406496ebc5b14731e4575f770563ddef21`  
		Last Modified: Tue, 05 Apr 2022 06:34:41 GMT  
		Size: 290.6 KB (290637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf30d07056a9a35092dc8a190963a5d19c14fce0543c6f6cfed98fc9a687dc5f`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bbde61fe85af3ebca0218d5ca1f9b5b6d095a57aedc0d7a827ba511e2143629`  
		Last Modified: Tue, 05 Apr 2022 06:34:48 GMT  
		Size: 11.1 MB (11106715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e9e55ef38253194b94160973edf2d58fbb2df74561e28d5e7894a3865f9daf8`  
		Last Modified: Tue, 05 Apr 2022 06:34:40 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:e526f540c45973c7a3a4585918890beceac9f0916e124daea3bf4e8b7a1e09b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13753199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2982d1a58becf38a1cf55541dcd74c1b096e8a02bb2060c30540fd3246e46e4f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 03:11:38 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 03:11:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 03:11:41 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 03:11:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:11:44 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:11:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:11:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:11:47 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:11:48 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:11:49 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 03:11:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:11:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:11:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:11:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:11:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:11:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:11:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:11:57 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:11:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:11:59 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:00 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b907f83114020e794129b34363890abf552785b8d964dbd3546272cc805702ce`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 291.3 KB (291281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988559859d9a4661992cbcefddba5b3d7a16de6c22547a962024f04767e6debf`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 5.7 KB (5748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7769260cde91250d6c68897788b078fea0a63b1254082d2923affeb859224a92`  
		Last Modified: Tue, 05 Apr 2022 03:13:22 GMT  
		Size: 10.7 MB (10738627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0143e63583cae9b0bc2b0048073b6c52476761cbeffa8e6aeca59d227ae0ee2`  
		Last Modified: Tue, 05 Apr 2022 03:13:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:0f4502864c2fae9298130a48ec4ca4351af0787bee15fd4cb5307b7b83e87dd8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13416150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b308dba8382e868224f828f88958151f9c1af01332da44ca296967f8bf09d40b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:44 GMT
ADD file:0b9367758b91930d9d69fd3901262e3a696f7a9f6d9e209e35da83ea6e785837 in / 
# Tue, 05 Apr 2022 00:23:46 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:07:02 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 07:07:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 07:07:12 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 07:07:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:07:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:07:29 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:07:31 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:07:33 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:07:36 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:07:40 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 07:07:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:07:45 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:07:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:07:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:07:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:07:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:07:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:08:03 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:08:06 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:08:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:08:10 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:08:12 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:ee5f6345565e7aeda814a5c097612cacb0a74186b1f01bf5199e1b812b5d3065`  
		Last Modified: Tue, 05 Apr 2022 00:25:06 GMT  
		Size: 2.8 MB (2814167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8affbe739a71e3875810f257750034ec7a6ee3f2f2c0094f3bcb3ed8a45520b`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 293.7 KB (293710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc927cb41936aaa5bfefa5dc4d654b7193fd568f619707120a5491c620906fc1`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8646c35213c358f518a4d76b75742b5930acec5d12cbd6c75d0a7e217698cee`  
		Last Modified: Tue, 05 Apr 2022 07:11:06 GMT  
		Size: 10.3 MB (10302288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346269e52424a62ec14d10c3e1db1aeb9cefe58f0bf6021855044138396bc074`  
		Last Modified: Tue, 05 Apr 2022 07:11:04 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:4bdb0834a42c22fa543fe4497215113db9aa55197d55597fb16c6cfd2a7ec22a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14225578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea0631ff02e5e01fcee0ebd5387c53f8dca8198463556fd98f569e3454b0bab`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 06:19:18 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 05 Apr 2022 06:19:20 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"
# Tue, 05 Apr 2022 06:19:20 GMT
ENV CADDY_VERSION=v2.4.6
# Tue, 05 Apr 2022 06:19:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='ecdcf8ecf6ba92032b27bc935e3ca18b192b25ff54ecfc26bc685ac71c6fe66a6d387cfd085d786533e20f3df3db86e18709a9556d86f1745e9358cc0984973e' ;; 		armhf)   binArch='armv6'; checksum='7d14b1a14a632fff0d82c6e8621c729319befa36b9be9ed2d0309170818e484b8280df4c78538460697afdec59f9781365cc89ac9183310bf15370d56d37ec28' ;; 		armv7)   binArch='armv7'; checksum='c5bc52232ce5cd8f4d91e03996cce9404568804fe6f0e97e79a2d595cadc21918b45fc9c7bc5b4da50a8e02f865391de39ececdeda30dfc592d8f3a5bda6e289' ;; 		aarch64) binArch='arm64'; checksum='c521f56e6332bb51fb5b9df9c6b790d3a1dc64731ac71bca8d798681b40d912ca54b70f64438efd7e7c926a7a3f7f4daf674080b5be9bfb6bb648238aaba09db' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='22b20f463c0b5963165fa26c29d3cd30518b85ab3ed1a2f3104c708abc0690b18bacb0ba3f0468ad58bee41472f01d2f9a37fa67a23b422b0070f76c38f3c667' ;; 		s390x)   binArch='s390x'; checksum='949f31cd4a9117c5ac23f195f5d50968ac3cd0cfa6ac3d7040c662a4a39679642f36cb42d9185f502e9887b147628e2c5dc402a06d01f00552a5ba9dfe774f09' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:23 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:24 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:25 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46276fc79092fffc5c0d503ca8733315c8e4002c4e7da79b2383f14c70565746`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 291.8 KB (291788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2e4510a7572a45fad3f051c23678f720057b3bb38d17381f62903aa621c6eb`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf64cfe3d9d0d01f6a1856e4850cd31a634fbb44641472deac6358fdc04352ea`  
		Last Modified: Tue, 05 Apr 2022 06:20:34 GMT  
		Size: 11.3 MB (11323733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363873546085e9612ff25fa067fed8e0038220696a865e645e8046a79035fc99`  
		Last Modified: Tue, 05 Apr 2022 06:20:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:984e29523be42ac2ec690474aeff5306ab5486f03150fc253c24474135df4522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:ab15bd89ffd1f282270324d942946ea48133d6d440d24e4f827d8eb6158d70d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2728749426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d0b9fff87adde7aa489199848d4b318b4767b67e5ec15d65b108a7a50bc2515`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 02:34:08 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:38:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/2f23e8a67eba98613ba87f2d04768f6b28875386/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 13 Apr 2022 04:38:49 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 13 Apr 2022 04:39:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.6/caddy_2.4.6_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('08fe8b50664644f5672a7357a7fe4c4835828c2464965ad78ec5f483dd2cd5643c64ea929d2f131601c48d71d2ddaebe251eb608d435ae1e31abe39d0687aebb')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:39:55 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:39:56 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:39:58 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:39:59 GMT
LABEL org.opencontainers.image.version=v2.4.6
# Wed, 13 Apr 2022 04:40:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:40:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:40:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:40:03 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:40:04 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:40:05 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:40:07 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:40:08 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:40:10 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:41:00 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:41:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba1c113303b8371787710ec139807b93d58a8b0789523fc35afdb65f6e94bc61`  
		Last Modified: Wed, 13 Apr 2022 03:15:12 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8129805e9e333a66c903463c3cbf8ee34716da4665df9a65dd4176eba5c5f06`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 378.1 KB (378101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0c02055157e86962dc990aa9eb8a76310c871f5a61b31fc28d4697c3db8027`  
		Last Modified: Wed, 13 Apr 2022 04:49:35 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be26f98c294634104232cfdf7721d86156da5170d2f782c70bae4574bb587dac`  
		Last Modified: Wed, 13 Apr 2022 04:49:47 GMT  
		Size: 12.1 MB (12129431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe26860d4106128398c2e4244c616de9b3f6775c09d7977cbdbf7e07d3e4350`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbfaea325a641b516609144f9457155163bc303f92dc2b46bf3234dc2bc3f6ba`  
		Last Modified: Wed, 13 Apr 2022 04:49:34 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9857ad4a90b4d3fbbe8a54858fc33b856253c82df5946008b54c9020ff97a8`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa2a0791f598311b730296aadf5765dfe4d8b6652e3c0f186a3704803484636`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5c96a870ea81640d2fca62d48afabb6c4df915a170f3167fd2f0a058783757`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690561b8f779dea8a5e958928913bf40a2e324743b44cf2148d0058450a9370e`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ce0ade7e6a82a8964ffe81d6f5cea0d637073ce7aa2d252c00aa56d2b81dcd`  
		Last Modified: Wed, 13 Apr 2022 04:49:32 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505081250451e81d15e6c1eac12af0dbde38f0fb87f0694c2d3ea17f9ba5a28d`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2f05c6016921246c90c6f9e626e461b5154f61ab3ace133bb77e495c693637`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997eb7f0df65fd16500f6a8101071fc5282bc2a6214fba537d3c7ffab7ed6486`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fe99a851b42e9ceba16ed5fabbf1a3eda63ec20fdb4cd1d22c11c185c95428b`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e0e4d528f07026bf00fb069474d1ee9406def0b2ad6a60ae034c13cff22ea82`  
		Last Modified: Wed, 13 Apr 2022 04:49:30 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9243d64b2a868795b63d1687c73d8944a331953f6bc8c987a811773c46a0fa03`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f824b9ab108252ee5eb3ea17f15ad21d529bfdea4481fe8360f08b491168c85`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785ba6d803e7c5e7f8037d8446b6f8074dd7a7e80dcef9381c785f1c2df4405f`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92658d6af13e1caa8bd3200ca2241b8406b49d4e7531ad59ad1268905619d377`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 296.1 KB (296128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d2ee45b3fb157613f5eb49f67c1657d107530b573c66cc50a33c338b835384`  
		Last Modified: Wed, 13 Apr 2022 04:49:28 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
