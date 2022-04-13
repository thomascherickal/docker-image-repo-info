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
$ docker pull caddy@sha256:14036c05891d952e4fb956693c2c63e50408107ad7507f524cd0ba883f1bb6b5
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:e53c62d8939d3f0bb4c1ed28923d80f7e07dc3912b5a39d0476db918358cfa1f
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:14036c05891d952e4fb956693c2c63e50408107ad7507f524cd0ba883f1bb6b5
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:e53c62d8939d3f0bb4c1ed28923d80f7e07dc3912b5a39d0476db918358cfa1f
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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

## `caddy:2.5.0-beta.1`

```console
$ docker pull caddy@sha256:beabdf1a66000dfde0b795f8d4cfa2c625bfce5c6376f39d1bd9758845936331
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

### `caddy:2.5.0-beta.1` - linux; amd64

```console
$ docker pull caddy@sha256:bac7580bfb78e7d7aedf9044ff33ba0a461e236bbe724253240722a2c2833b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15281277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4004608d8af3d2fb6ce0c5961777a4106636aa68d2ed9809df92c5b85acff4`
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
# Tue, 05 Apr 2022 04:25:01 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 04:25:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:25:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:25:07 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:25:07 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:25:07 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:25:07 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:25:08 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:25:08 GMT
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
	-	`sha256:e05594f38e13e9c731a8ab55b382f8af8c26f09320e016462a84c4f7ea29b09a`  
		Last Modified: Tue, 05 Apr 2022 04:25:50 GMT  
		Size: 12.2 MB (12169217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c7da94e5fbe8d331bb4363cff609ee7a5af046d180358dfdb9745ba19a2c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:995e1ee69c4e941859c8fe08ee8c7ae5d7e449f4e5243d0618391c04353271f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14451284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f8e1c5a4506d1ba5fe3ba7e360fe1bdd8a8668ceb8306da0e02fae7ba993e2`
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
# Tue, 05 Apr 2022 03:15:04 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:15:11 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:15:11 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:15:12 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:15:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:15:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:15:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:15:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:15:15 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:15:16 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:15:16 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:15:17 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:15:17 GMT
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
	-	`sha256:150950fa1b63c40e7ca5764cdeb7988d8a15f550762999723e6e9659c38282c5`  
		Last Modified: Tue, 05 Apr 2022 03:18:18 GMT  
		Size: 11.5 MB (11531644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b85c24743ba55b919e1a0b33c9589948cbef4830c588108e9698ce11235633`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:64dcd6e2cc4aad2c2c89bb7cded9819935056ee5c8aaa4f9ef182bc356435ff1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946580d1e058d0c7451feaf278c204e5bc0da968acf3f2807928c02b8fbcdbd9`
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
# Tue, 05 Apr 2022 06:33:08 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:33:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:33:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:33:14 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:33:14 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:33:15 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:33:15 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:33:15 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:33:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:33:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:33:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:33:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:33:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:33:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:33:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:33:19 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:33:19 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:33:20 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:33:20 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:33:21 GMT
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
	-	`sha256:8cfc5deee1bf6f6600fe8402d08138fbf5fb1e9132ae3e820cb274ff78de74c0`  
		Last Modified: Tue, 05 Apr 2022 06:35:15 GMT  
		Size: 11.5 MB (11511975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c950586adcccfcf1ec15e40da0fb338ab975c2f6d63a3f49fbd43ab5a6b9b6`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:99a7c0298ba26e39221504632853f0c12b3cc6d51ebf1d957a8614c2ac62298f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14151675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181d197c22004b9c4242984dee400be86b249372bad74740eb818cc9febf0be6`
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
# Tue, 05 Apr 2022 03:12:17 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:12:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:12:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:12:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:12:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:12:24 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:12:25 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:12:26 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:12:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:12:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:12:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:12:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:12:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:12:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:12:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:12:34 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:12:35 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:12:36 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:37 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:38 GMT
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
	-	`sha256:d5e0ff4c04fc65e4d2e778c739fe0dff0ca9b8006b0ea5e71af2210c38c1ef87`  
		Last Modified: Tue, 05 Apr 2022 03:13:41 GMT  
		Size: 11.1 MB (11137996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52cf9a10ab3f4c966798e5ce44cc9569cc31658785767c0d438f7a435666f055`  
		Last Modified: Tue, 05 Apr 2022 03:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:98a632b2c106991170be442d14b4ed3db078616bd2c5787604c1688ea46b5af0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3e24a28142e386eb1c4b37b83e291e4256a3f481e3a354f3b4bd160d8156c5`
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
# Tue, 05 Apr 2022 07:08:45 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 07:08:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:09:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:09:06 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:09:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:09:11 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:09:13 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:09:17 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 07:09:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:09:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:09:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:09:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:09:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:09:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:09:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:09:55 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:09:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:10:00 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:10:04 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:10:06 GMT
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
	-	`sha256:e79976b8a08e399f4d6fd3eb19500adbb418be5088bda898ef58f47c6791c2aa`  
		Last Modified: Tue, 05 Apr 2022 07:11:26 GMT  
		Size: 10.7 MB (10675672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6866f1a9b35b79bf3c4b8bf13c2c2d5b1ffd33351937a641fc88f72ed011a0a7`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - linux; s390x

```console
$ docker pull caddy@sha256:5dc3ae5b9a9ec370660f1a192517138ca1f1822436e05f51f2cfd7d8969c901a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14627648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e041975d62fa3de352fb55c2d7349d1f7a023f98d76da64f25a9ef635bf442a`
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
# Tue, 05 Apr 2022 06:19:42 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:19:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:45 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:45 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:45 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:45 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:46 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:46 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:47 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:47 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:47 GMT
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
	-	`sha256:62d9efb35d6033b2097e2b43f03270f6509c549e025a79566426a0c5e9450cf6`  
		Last Modified: Tue, 05 Apr 2022 06:20:46 GMT  
		Size: 11.7 MB (11729468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f7e89e0dae073ed741dd140b8085f3e69a24baa02f5c4e762e24aece4e7d5e`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:6e626bf72e437a353d6d01d85f56a7ab74163cd1f9ca5132b70cc81b0ac95091
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729197641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2933cead23078da080b488af18ccea0fa4fcfe7157e8c7ed24eb9100f40e87`
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
# Wed, 13 Apr 2022 04:42:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:43:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:43:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:43:47 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:43:48 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:43:49 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:43:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:43:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:43:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:43:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:43:57 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:43:58 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:43:59 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:44:58 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:44:59 GMT
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
	-	`sha256:6f22b56b6abc68d2c947d2a5b077ed0ed9d7b9b281a92de72c0b337a88f7f52b`  
		Last Modified: Wed, 13 Apr 2022 04:50:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c010d9d46a653c0e43534061f409f08fc8276e27bf12dc32f301d0522851c72c`  
		Last Modified: Wed, 13 Apr 2022 04:50:32 GMT  
		Size: 12.6 MB (12577776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a0d3443230920064e9a4ad603b313c3c112274675ee2d708845c31b01dff9`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8ec8f791c42c04c3ef9e9f63a6b263171412c7e653edbfa0da0ec5e302bbd`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d680fb76d896678fdd8db202fd05ccef68bc5dac499f1bb879a7afb9187fba`  
		Last Modified: Wed, 13 Apr 2022 04:50:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63775f08de58cfb563826ceb049f60eefecc09543520658d8c477b46ea054366`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d1ebc23d80d71f3f4c63af582cd73aec506328e3161ad08e6e22c3f3b1c631`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3070fa2a1cb5b58c6fc3d98dcf6dfe4190d619f757eaa321ae732ce5bdcb23`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cfe04dbc46bdb60c88f0aef2f22d16ddca431bbcfcbe8f9e54484a919e63ed`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612434bf8a03dd5fd2c666445bcf8e738df97316a3cfbf971751f10dada6e630`  
		Last Modified: Wed, 13 Apr 2022 04:50:25 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892e35d6a0cb734d147c4857708dd0da7717e8d3313f67b4243d3a1cc88ed3d`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4271146ce30c8ec1371049216f34f5c896cad13bd8c2d125dfb307d68c20ba2`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bb125793433dd4c894875a1e1df0c00563c6773d50227c6887bcee5ab962d0`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d551fc39269de6a08e0405be92b691b0a0c5e1add58f6e8cb1d1aa745845bb5`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd140311bf4ea4dda888642ca6d59e45279eca51b08fe5537dde2aa55b706ba`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14735299e19c40b09e06312a6309062c1984f1ba31f31392632fb498712e4978`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384b686208549fdef850ba3c8633261fc7fbbc96e758b0796f41addc40a1896`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811878d9e084fbf7c4d4c08d3f5d62c128d14cf147703b400436417f6a2e25ac`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 296.0 KB (296004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072405dc4b79db0e852b35ceb62ef6f2252c4322a430df8f44a50e9767e0c235`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:e3a8016c3c64a49897996ad69c0325e61752cdbc9ca844fa697f910bec8c98ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240771001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6e2b2b1ff8bf31f17438be13c2da7d529f76fcbe313e4eed06b9bc69f5d318`
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
# Wed, 13 Apr 2022 04:45:43 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:46:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:46:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:46:13 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:46:14 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:46:15 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:46:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:46:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:46:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:46:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:46:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:46:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:46:23 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:46:24 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:46:25 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:46:42 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:46:43 GMT
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
	-	`sha256:2e7d68c69939c53f016e8cf0d51d57a2b78dfcc512d66e66d6d2b4cb5a7f57b8`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f3727ab2382f41b18d95c8da347a7c755809b2191bf9f6a2fa46c171515824`  
		Last Modified: Wed, 13 Apr 2022 04:50:48 GMT  
		Size: 12.8 MB (12806637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dbb4d1a1e66edfd4b8227a146c73da1c1a5b984b7a709077d3df2b4619ed36`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25797b5f8af5b9846b486d46533da312930f863dca5d535061c13ac714cd8ec3`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccad74ccb9c577bc14a32134581b3f7d84f337fff019f4731b2a5f0c2c4b3f3`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c417f50c24094ea52e14331102360f4b3dd1b9f45719d1958f213f7ba645a5`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8fe45f94b2a2a75ff87a852e62b4fa9d18e5957365a0f3bfef85ee6da438f`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385801886c7f0293ab1b4b73193694ba1894a073b2ca5bf6735ba6ab16e34bc8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7d3e8a14bd7be12c7cbe40179fe5629f9446304feaadd2ab05fd465a0d3fd8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b92f30c475135a743a6752551f98a419b50f1ac541986c70339f36893f594f`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e80373ab79d4bd62bdd7971eb48f57334a2ce9ebd003647793e8a42025a7da8`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894294ebbe0380c696560955ca8e7b4007a9755305d872a7a08d2826f22ae734`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f6cd0e22f9513b18449e31ca425f5df0953cfb3e871179d34fd0fda91f728`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd68b9283a3e645eb13d6bf37b082a6405d6206ec33a1d9b8d57517c1d7dad23`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ec800f2a4638585b430b77da5a02fe8e5d739ae72a39869b2245eb7a8d8c6`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1671c65a57df30824e5058cf7fd6ac03442647e39234294e645cfd8f47c4a959`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c7e95b436b0a98f22b75bd760de1d59cef1cd2ecc16bd210204594698f727d`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cffba02c62a0ebbe70a3c5df4dacaa4054a9fcecc3b0c0a9d53896c6095e01e`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 346.0 KB (345957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2062b0d139ab02b47e030fb1a8980c3f3f86925f74de2fca500b7bc1f226a357`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-alpine`

```console
$ docker pull caddy@sha256:bd9bf209e694c63dbfb34f04547c62c8fb4c5afca702f2674d551b3163e63864
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
$ docker pull caddy@sha256:bac7580bfb78e7d7aedf9044ff33ba0a461e236bbe724253240722a2c2833b37
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15281277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f4004608d8af3d2fb6ce0c5961777a4106636aa68d2ed9809df92c5b85acff4`
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
# Tue, 05 Apr 2022 04:25:01 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 04:25:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 04:25:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 04:25:07 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 04:25:07 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 04:25:07 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 04:25:07 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 04:25:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 04:25:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 80
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 443
# Tue, 05 Apr 2022 04:25:08 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 04:25:08 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 04:25:08 GMT
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
	-	`sha256:e05594f38e13e9c731a8ab55b382f8af8c26f09320e016462a84c4f7ea29b09a`  
		Last Modified: Tue, 05 Apr 2022 04:25:50 GMT  
		Size: 12.2 MB (12169217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c7da94e5fbe8d331bb4363cff609ee7a5af046d180358dfdb9745ba19a2c1`  
		Last Modified: Tue, 05 Apr 2022 04:25:48 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:995e1ee69c4e941859c8fe08ee8c7ae5d7e449f4e5243d0618391c04353271f7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.5 MB (14451284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f8e1c5a4506d1ba5fe3ba7e360fe1bdd8a8668ceb8306da0e02fae7ba993e2`
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
# Tue, 05 Apr 2022 03:15:04 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:15:11 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:15:11 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:15:12 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:15:12 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:15:13 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:15:14 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:15:14 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:15:15 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:15:15 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:15:16 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:15:16 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:15:17 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:15:17 GMT
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
	-	`sha256:150950fa1b63c40e7ca5764cdeb7988d8a15f550762999723e6e9659c38282c5`  
		Last Modified: Tue, 05 Apr 2022 03:18:18 GMT  
		Size: 11.5 MB (11531644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b85c24743ba55b919e1a0b33c9589948cbef4830c588108e9698ce11235633`  
		Last Modified: Tue, 05 Apr 2022 03:18:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:64dcd6e2cc4aad2c2c89bb7cded9819935056ee5c8aaa4f9ef182bc356435ff1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14232949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:946580d1e058d0c7451feaf278c204e5bc0da968acf3f2807928c02b8fbcdbd9`
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
# Tue, 05 Apr 2022 06:33:08 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:33:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:33:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:33:14 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:33:14 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:33:15 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:33:15 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:33:15 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:33:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:33:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:33:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:33:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:33:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:33:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:33:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:33:19 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:33:19 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:33:20 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:33:20 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:33:21 GMT
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
	-	`sha256:8cfc5deee1bf6f6600fe8402d08138fbf5fb1e9132ae3e820cb274ff78de74c0`  
		Last Modified: Tue, 05 Apr 2022 06:35:15 GMT  
		Size: 11.5 MB (11511975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84c950586adcccfcf1ec15e40da0fb338ab975c2f6d63a3f49fbd43ab5a6b9b6`  
		Last Modified: Tue, 05 Apr 2022 06:35:07 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:99a7c0298ba26e39221504632853f0c12b3cc6d51ebf1d957a8614c2ac62298f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.2 MB (14151675 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:181d197c22004b9c4242984dee400be86b249372bad74740eb818cc9febf0be6`
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
# Tue, 05 Apr 2022 03:12:17 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:12:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 03:12:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 03:12:22 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 03:12:23 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 03:12:24 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 03:12:25 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 03:12:26 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 03:12:27 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 03:12:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 03:12:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 03:12:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 03:12:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 03:12:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 03:12:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 03:12:34 GMT
EXPOSE 80
# Tue, 05 Apr 2022 03:12:35 GMT
EXPOSE 443
# Tue, 05 Apr 2022 03:12:36 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 03:12:37 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 03:12:38 GMT
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
	-	`sha256:d5e0ff4c04fc65e4d2e778c739fe0dff0ca9b8006b0ea5e71af2210c38c1ef87`  
		Last Modified: Tue, 05 Apr 2022 03:13:41 GMT  
		Size: 11.1 MB (11137996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52cf9a10ab3f4c966798e5ce44cc9569cc31658785767c0d438f7a435666f055`  
		Last Modified: Tue, 05 Apr 2022 03:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:98a632b2c106991170be442d14b4ed3db078616bd2c5787604c1688ea46b5af0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13786562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df3e24a28142e386eb1c4b37b83e291e4256a3f481e3a354f3b4bd160d8156c5`
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
# Tue, 05 Apr 2022 07:08:45 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 07:08:53 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 07:09:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 07:09:06 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 07:09:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 07:09:11 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 07:09:13 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 07:09:17 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 07:09:20 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 07:09:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 07:09:26 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 07:09:31 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 07:09:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 07:09:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 07:09:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 07:09:55 GMT
EXPOSE 80
# Tue, 05 Apr 2022 07:09:58 GMT
EXPOSE 443
# Tue, 05 Apr 2022 07:10:00 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 07:10:04 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 07:10:06 GMT
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
	-	`sha256:e79976b8a08e399f4d6fd3eb19500adbb418be5088bda898ef58f47c6791c2aa`  
		Last Modified: Tue, 05 Apr 2022 07:11:26 GMT  
		Size: 10.7 MB (10675672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6866f1a9b35b79bf3c4b8bf13c2c2d5b1ffd33351937a641fc88f72ed011a0a7`  
		Last Modified: Tue, 05 Apr 2022 07:11:24 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:5dc3ae5b9a9ec370660f1a192517138ca1f1822436e05f51f2cfd7d8969c901a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14627648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e041975d62fa3de352fb55c2d7349d1f7a023f98d76da64f25a9ef635bf442a`
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
# Tue, 05 Apr 2022 06:19:42 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:19:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='4624dd27b7b53a0b82e17bfb64901eece99ffd943af888f3815e20e0b55c1aaadc15c6f517d985ffcf911e21ef9cb78a044661407a6d4e3c543f2cceede53f7e' ;; 		armhf)   binArch='armv6'; checksum='8615a6aacd10cb2e74f169ae1756ecd8508521791e511f8eca0dfc05f312aae5822b209787f4917c722a01e943f9317b35c8aa436c9086239e564079ef270078' ;; 		armv7)   binArch='armv7'; checksum='dc7c70efaaed0df7c6af959dd61ce79cae8d1217c6a8a68196eaef92438bd51a019f40dbc4e2f112c8ef8d01312d2e7bc8efc40d5e91342b8dba78ed2407e7da' ;; 		aarch64) binArch='arm64'; checksum='50065feb4b20f1c6f2fb4305047f8cd5eca8eb6dae478944c93078402905513c715c5bbbad43a3c90a766c6b75bb18de53023a8e07238733d6436a8a18960162' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='c36537aa861ae9bb41db661ed8dd2e04c1904bd25a0d600b5ee2aa94f8ab7724bc3003e8708f7a41204b42d30b80b53e9655f0bf8fd91bfea36f75d5ddd76534' ;; 		s390x)   binArch='s390x'; checksum='26d6be36fb481e2483308cbd97a20b1c1ebc4d332157b9ff440edb33f825787cd205bf5f5a2fdaef1c214fb8a3c2a497db8fd8b58844d885d83f223f119c4034' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 05 Apr 2022 06:19:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 05 Apr 2022 06:19:45 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 05 Apr 2022 06:19:45 GMT
ENV XDG_DATA_HOME=/data
# Tue, 05 Apr 2022 06:19:45 GMT
VOLUME [/config]
# Tue, 05 Apr 2022 06:19:45 GMT
VOLUME [/data]
# Tue, 05 Apr 2022 06:19:45 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Tue, 05 Apr 2022 06:19:45 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 05 Apr 2022 06:19:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 05 Apr 2022 06:19:46 GMT
EXPOSE 80
# Tue, 05 Apr 2022 06:19:46 GMT
EXPOSE 443
# Tue, 05 Apr 2022 06:19:47 GMT
EXPOSE 2019
# Tue, 05 Apr 2022 06:19:47 GMT
WORKDIR /srv
# Tue, 05 Apr 2022 06:19:47 GMT
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
	-	`sha256:62d9efb35d6033b2097e2b43f03270f6509c549e025a79566426a0c5e9450cf6`  
		Last Modified: Tue, 05 Apr 2022 06:20:46 GMT  
		Size: 11.7 MB (11729468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f7e89e0dae073ed741dd140b8085f3e69a24baa02f5c4e762e24aece4e7d5e`  
		Last Modified: Tue, 05 Apr 2022 06:20:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder`

```console
$ docker pull caddy@sha256:27ceb14b0de77b5e67089e5401ac513d8f0aeda13525b1ef4a26c6c2544ea7a0
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

### `caddy:2.5.0-beta.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:aa8bfcbcd8d143b74cc0bf2ea14bc6e857d5d5288843ec348ee51716e83e7dc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abcc67abbacee168f203e6debce07c1f89936f105c7096b22cd7b15eab62ffcb`
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
# Wed, 13 Apr 2022 02:49:19 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 02:49:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:20 GMT
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
	-	`sha256:db0a51b54bacb7d433e4ade0e08b0cb792ef5d2a72ec9cf93534f658fb2285fb`  
		Last Modified: Wed, 13 Apr 2022 02:49:54 GMT  
		Size: 1.2 MB (1245713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2fa190d341837711e2b8cea86776918f61758ef38d9a44f2c0135cf5ef397b`  
		Last Modified: Wed, 13 Apr 2022 02:49:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:919545d0e99e839b366d5d5b26eea0fe8dfd5ea0bc8ba790359b9397bc88956b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b27fa32518228601cfe30c59f76450b0d0a71d504d3f1d2b0e19dca3acbd40`
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
# Wed, 13 Apr 2022 03:29:09 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:29:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:29:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:29:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:29:13 GMT
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
	-	`sha256:21b7c0509892927652d6a3d1a9a084eaf72382e1d4b50164cde5dc97fcd02c92`  
		Last Modified: Wed, 13 Apr 2022 03:30:48 GMT  
		Size: 1.2 MB (1178512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601e92075dcad4e5c08ba5c062d03effb617f98154763a6303371598bcf1a211`  
		Last Modified: Wed, 13 Apr 2022 03:30:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:46e8de3418b30e4d0c73091f48ca7272af113b2231827d181058c0690299cfbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15a48ed4c6ddea63b63907d7e1139163787fc1a4f2dcbd1f02d35a9970f7258`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:58 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 06 Apr 2022 02:23:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:24:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:24:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:24:01 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc619e37ad9461e5adce59223051ac7835d62f4ff59ec13dd09cc8fe03386bb6`  
		Last Modified: Wed, 06 Apr 2022 02:25:38 GMT  
		Size: 1.2 MB (1176714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4be834d337fe68ed4f43831e9e9969f38dd4283be0aec04d58c2a9f9d54e81`  
		Last Modified: Wed, 06 Apr 2022 02:25:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c456d6beff9f57282ef28114d01d2b1ca242e14bc2adf1a0cb3f64905a3b724b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4ac001421bea79c22ff9cfc8dec1b13428a2868eaccf77d2a3948719ba8644`
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
# Wed, 13 Apr 2022 03:10:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:10:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:41 GMT
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
	-	`sha256:3cb588ae109f91fa709ab5bd5f9e2b32166d76b3ce44c7d8fd36097400595b37`  
		Last Modified: Wed, 13 Apr 2022 03:11:34 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbab1968da74a5890834e85455685a6290b2efd7fbfd669f63e1c828582c370`  
		Last Modified: Wed, 13 Apr 2022 03:11:33 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:c44d453fcb8d17c94d390003e2815659dbf19c9ce5486236f2f779784c1ad5dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623a6b20bc2d6225bddc47894538e88655474ebd1bc8603bdb94a5778f0f2937`
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
# Wed, 13 Apr 2022 03:16:06 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:16:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:16:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:16:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:16:24 GMT
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
	-	`sha256:8508eb2e1cd4ded98b1a0fc63eaad865bf7f4b8c149fe7e81b9477264b5392f1`  
		Last Modified: Wed, 13 Apr 2022 03:17:26 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a434c821a25bc78fa015865cde6889aafb54bbde5607c272a67521a46b8deb`  
		Last Modified: Wed, 13 Apr 2022 03:17:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:115feb502aa0b4c7b88154c2cfe103dd84b194dad2ec8bf1c32707f771a153d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad2ccde491039fc520253533cff099a3be7e246bc01e58422267ccf296d6e6d`
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
# Wed, 13 Apr 2022 03:13:06 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:13:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:13:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:13:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:13:08 GMT
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
	-	`sha256:53f25bad0652c60861b53eb4094e149460b962355a6db19b9599a2c330f7eb57`  
		Last Modified: Wed, 13 Apr 2022 03:14:00 GMT  
		Size: 1.2 MB (1203780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438ed41be20bb524dec662a88eb5897ff01fbf5ce2f8ae0afa254aaa7820e0c3`  
		Last Modified: Wed, 13 Apr 2022 03:14:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:771215ec207c454093ac0c634172b5cd5973571c6802d3cf5639f723ece02201
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0055d3ad15ef34d8f54604abcccb88109fcf272e3acc6a2587ec04a784a9a2de`
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
# Wed, 13 Apr 2022 04:47:02 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:48:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:48:09 GMT
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
	-	`sha256:4cfcb0e1a33c91121ca576dad4ed65382260da99a6321393b4c84087425dae90`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc85786aa07e11a03dfbed28810a2765d7e53350daeffb34b7a09761cfe399`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9464f4b73282195e824ebaa0454b32e372c954812b09242ed4f5c87aa58bf0aa`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.7 MB (1661509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781d1939a654d2f7b612983f19bbf73fe2bc37226e6b2768f68c71b4593d5d7b`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:988edc26e9cb78977c3859b52b03e2491e58784a555a162d7db9eac6c72cfa9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2400912866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b94c72984c4f20638cabedc32e3ce0d9390727d560fdd7780fde3bd9bc742c4`
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
# Wed, 13 Apr 2022 02:51:52 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:55:12 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:55:14 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:48:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:48:17 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:48:18 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:48:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:48:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:48:49 GMT
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
	-	`sha256:9260daf825796a9195ffeb15e5b68094166214dea8388c7249c46d5ab4599377`  
		Last Modified: Wed, 13 Apr 2022 03:19:18 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b5fe72bfea25d1314ca3d3217699ab16f59bed8b459f195126ba4815bd3d75`  
		Last Modified: Wed, 13 Apr 2022 03:20:13 GMT  
		Size: 145.8 MB (145767213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8075970b46df5ae0331f5cede49b2eb4110ebdbc0d8e171ab0f7f8aa8a70ce5c`  
		Last Modified: Wed, 13 Apr 2022 03:19:18 GMT  
		Size: 1.6 KB (1564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae0f3b52ca6a6aabd2fe3ce81fa9d04e01af3417015efd039e1810abf873983`  
		Last Modified: Wed, 13 Apr 2022 04:51:06 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0715e2766695446843c7bc3af26e4e2c9fa4cbd7176d3d094087186cdeed7e`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40c691059116c5ce841d43668e92774a1440c38bde8a9853770d089e1e735e`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e5c70137b535fd6bcc705cad6ffc0e860deade0a6c7b26dbab5b04784f1ce1`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0137263350e51f0064902031730a9acf956e4c99e624ee0d5b16602e803d1c6`  
		Last Modified: Wed, 13 Apr 2022 04:51:06 GMT  
		Size: 1.9 MB (1895502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fde2bfc2e8282838e8849993c828dff3b3cf08854f5cd6751ac1474d8c4971`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-alpine`

```console
$ docker pull caddy@sha256:9a8ee965454f364474d0db0b94c39b079a04d6708618a84f988b38886afdda3d
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
$ docker pull caddy@sha256:aa8bfcbcd8d143b74cc0bf2ea14bc6e857d5d5288843ec348ee51716e83e7dc4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121396236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abcc67abbacee168f203e6debce07c1f89936f105c7096b22cd7b15eab62ffcb`
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
# Wed, 13 Apr 2022 02:49:19 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 02:49:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 02:49:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 02:49:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 02:49:20 GMT
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
	-	`sha256:db0a51b54bacb7d433e4ade0e08b0cb792ef5d2a72ec9cf93534f658fb2285fb`  
		Last Modified: Wed, 13 Apr 2022 02:49:54 GMT  
		Size: 1.2 MB (1245713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2fa190d341837711e2b8cea86776918f61758ef38d9a44f2c0135cf5ef397b`  
		Last Modified: Wed, 13 Apr 2022 02:49:54 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:919545d0e99e839b366d5d5b26eea0fe8dfd5ea0bc8ba790359b9397bc88956b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115827383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77b27fa32518228601cfe30c59f76450b0d0a71d504d3f1d2b0e19dca3acbd40`
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
# Wed, 13 Apr 2022 03:29:09 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:29:10 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:29:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:29:12 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:29:13 GMT
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
	-	`sha256:21b7c0509892927652d6a3d1a9a084eaf72382e1d4b50164cde5dc97fcd02c92`  
		Last Modified: Wed, 13 Apr 2022 03:30:48 GMT  
		Size: 1.2 MB (1178512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601e92075dcad4e5c08ba5c062d03effb617f98154763a6303371598bcf1a211`  
		Last Modified: Wed, 13 Apr 2022 03:30:47 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:46e8de3418b30e4d0c73091f48ca7272af113b2231827d181058c0690299cfbc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e15a48ed4c6ddea63b63907d7e1139163787fc1a4f2dcbd1f02d35a9970f7258`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:58 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 06 Apr 2022 02:23:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:24:00 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:24:01 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:24:01 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc619e37ad9461e5adce59223051ac7835d62f4ff59ec13dd09cc8fe03386bb6`  
		Last Modified: Wed, 06 Apr 2022 02:25:38 GMT  
		Size: 1.2 MB (1176714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a4be834d337fe68ed4f43831e9e9969f38dd4283be0aec04d58c2a9f9d54e81`  
		Last Modified: Wed, 06 Apr 2022 02:25:37 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:c456d6beff9f57282ef28114d01d2b1ca242e14bc2adf1a0cb3f64905a3b724b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115538900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd4ac001421bea79c22ff9cfc8dec1b13428a2868eaccf77d2a3948719ba8644`
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
# Wed, 13 Apr 2022 03:10:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:10:38 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:10:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:10:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:10:41 GMT
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
	-	`sha256:3cb588ae109f91fa709ab5bd5f9e2b32166d76b3ce44c7d8fd36097400595b37`  
		Last Modified: Wed, 13 Apr 2022 03:11:34 GMT  
		Size: 1.1 MB (1148676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbab1968da74a5890834e85455685a6290b2efd7fbfd669f63e1c828582c370`  
		Last Modified: Wed, 13 Apr 2022 03:11:33 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:c44d453fcb8d17c94d390003e2815659dbf19c9ce5486236f2f779784c1ad5dd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114374595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:623a6b20bc2d6225bddc47894538e88655474ebd1bc8603bdb94a5778f0f2937`
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
# Wed, 13 Apr 2022 03:16:06 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:16:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:16:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:16:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:16:24 GMT
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
	-	`sha256:8508eb2e1cd4ded98b1a0fc63eaad865bf7f4b8c149fe7e81b9477264b5392f1`  
		Last Modified: Wed, 13 Apr 2022 03:17:26 GMT  
		Size: 1.1 MB (1120843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25a434c821a25bc78fa015865cde6889aafb54bbde5607c272a67521a46b8deb`  
		Last Modified: Wed, 13 Apr 2022 03:17:26 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:115feb502aa0b4c7b88154c2cfe103dd84b194dad2ec8bf1c32707f771a153d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118779255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aad2ccde491039fc520253533cff099a3be7e246bc01e58422267ccf296d6e6d`
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
# Wed, 13 Apr 2022 03:13:06 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 03:13:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 03:13:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 13 Apr 2022 03:13:07 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 13 Apr 2022 03:13:08 GMT
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
	-	`sha256:53f25bad0652c60861b53eb4094e149460b962355a6db19b9599a2c330f7eb57`  
		Last Modified: Wed, 13 Apr 2022 03:14:00 GMT  
		Size: 1.2 MB (1203780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:438ed41be20bb524dec662a88eb5897ff01fbf5ce2f8ae0afa254aaa7820e0c3`  
		Last Modified: Wed, 13 Apr 2022 03:14:00 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:541ff3a8e92d39520482e2404b58665de3159b786f645221566149911d3594c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.5.0-beta.1-builder-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:771215ec207c454093ac0c634172b5cd5973571c6802d3cf5639f723ece02201
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2888960490 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0055d3ad15ef34d8f54604abcccb88109fcf272e3acc6a2587ec04a784a9a2de`
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
# Wed, 13 Apr 2022 04:47:02 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:47:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:48:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:48:09 GMT
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
	-	`sha256:4cfcb0e1a33c91121ca576dad4ed65382260da99a6321393b4c84087425dae90`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdc85786aa07e11a03dfbed28810a2765d7e53350daeffb34b7a09761cfe399`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9464f4b73282195e824ebaa0454b32e372c954812b09242ed4f5c87aa58bf0aa`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.7 MB (1661509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781d1939a654d2f7b612983f19bbf73fe2bc37226e6b2768f68c71b4593d5d7b`  
		Last Modified: Wed, 13 Apr 2022 04:50:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:efb4fb8a6cb28d318255d6921e1d5f3e24a83152fe4710af0b4ffc0a7bb4f5d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-beta.1-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:988edc26e9cb78977c3859b52b03e2491e58784a555a162d7db9eac6c72cfa9d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2400912866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b94c72984c4f20638cabedc32e3ce0d9390727d560fdd7780fde3bd9bc742c4`
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
# Wed, 13 Apr 2022 02:51:52 GMT
ENV GOLANG_VERSION=1.17.9
# Wed, 13 Apr 2022 02:55:12 GMT
RUN $url = 'https://dl.google.com/go/go1.17.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '82752c3313cc6c1e1b5d73743a3ec569b09a14246fc2cb0824cf30f9f42a6005'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 02:55:14 GMT
WORKDIR C:\go
# Wed, 13 Apr 2022 04:48:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 04:48:17 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 13 Apr 2022 04:48:18 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:48:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 13 Apr 2022 04:48:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('fc6f2a7feb8f0936a0e04d3c9ea26d0404c2f4907eb436eb60e33152c22c1211f851c46606573fcb5c3334f8cc4f7f810b28b917a9f313f6454d1c5cd0f50f8a')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 13 Apr 2022 04:48:49 GMT
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
	-	`sha256:9260daf825796a9195ffeb15e5b68094166214dea8388c7249c46d5ab4599377`  
		Last Modified: Wed, 13 Apr 2022 03:19:18 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b5fe72bfea25d1314ca3d3217699ab16f59bed8b459f195126ba4815bd3d75`  
		Last Modified: Wed, 13 Apr 2022 03:20:13 GMT  
		Size: 145.8 MB (145767213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8075970b46df5ae0331f5cede49b2eb4110ebdbc0d8e171ab0f7f8aa8a70ce5c`  
		Last Modified: Wed, 13 Apr 2022 03:19:18 GMT  
		Size: 1.6 KB (1564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae0f3b52ca6a6aabd2fe3ce81fa9d04e01af3417015efd039e1810abf873983`  
		Last Modified: Wed, 13 Apr 2022 04:51:06 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b0715e2766695446843c7bc3af26e4e2c9fa4cbd7176d3d094087186cdeed7e`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa40c691059116c5ce841d43668e92774a1440c38bde8a9853770d089e1e735e`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e5c70137b535fd6bcc705cad6ffc0e860deade0a6c7b26dbab5b04784f1ce1`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0137263350e51f0064902031730a9acf956e4c99e624ee0d5b16602e803d1c6`  
		Last Modified: Wed, 13 Apr 2022 04:51:06 GMT  
		Size: 1.9 MB (1895502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6fde2bfc2e8282838e8849993c828dff3b3cf08854f5cd6751ac1474d8c4971`  
		Last Modified: Wed, 13 Apr 2022 04:51:03 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore`

```console
$ docker pull caddy@sha256:f460a4d5c0354e5a7b95c0695aa066c0c4d928f055ada448a2023eb449faa925
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.2803; amd64
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-beta.1-windowsservercore` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:6e626bf72e437a353d6d01d85f56a7ab74163cd1f9ca5132b70cc81b0ac95091
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729197641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2933cead23078da080b488af18ccea0fa4fcfe7157e8c7ed24eb9100f40e87`
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
# Wed, 13 Apr 2022 04:42:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:43:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:43:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:43:47 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:43:48 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:43:49 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:43:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:43:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:43:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:43:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:43:57 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:43:58 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:43:59 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:44:58 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:44:59 GMT
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
	-	`sha256:6f22b56b6abc68d2c947d2a5b077ed0ed9d7b9b281a92de72c0b337a88f7f52b`  
		Last Modified: Wed, 13 Apr 2022 04:50:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c010d9d46a653c0e43534061f409f08fc8276e27bf12dc32f301d0522851c72c`  
		Last Modified: Wed, 13 Apr 2022 04:50:32 GMT  
		Size: 12.6 MB (12577776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a0d3443230920064e9a4ad603b313c3c112274675ee2d708845c31b01dff9`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8ec8f791c42c04c3ef9e9f63a6b263171412c7e653edbfa0da0ec5e302bbd`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d680fb76d896678fdd8db202fd05ccef68bc5dac499f1bb879a7afb9187fba`  
		Last Modified: Wed, 13 Apr 2022 04:50:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63775f08de58cfb563826ceb049f60eefecc09543520658d8c477b46ea054366`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d1ebc23d80d71f3f4c63af582cd73aec506328e3161ad08e6e22c3f3b1c631`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3070fa2a1cb5b58c6fc3d98dcf6dfe4190d619f757eaa321ae732ce5bdcb23`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cfe04dbc46bdb60c88f0aef2f22d16ddca431bbcfcbe8f9e54484a919e63ed`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612434bf8a03dd5fd2c666445bcf8e738df97316a3cfbf971751f10dada6e630`  
		Last Modified: Wed, 13 Apr 2022 04:50:25 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892e35d6a0cb734d147c4857708dd0da7717e8d3313f67b4243d3a1cc88ed3d`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4271146ce30c8ec1371049216f34f5c896cad13bd8c2d125dfb307d68c20ba2`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bb125793433dd4c894875a1e1df0c00563c6773d50227c6887bcee5ab962d0`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d551fc39269de6a08e0405be92b691b0a0c5e1add58f6e8cb1d1aa745845bb5`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd140311bf4ea4dda888642ca6d59e45279eca51b08fe5537dde2aa55b706ba`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14735299e19c40b09e06312a6309062c1984f1ba31f31392632fb498712e4978`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384b686208549fdef850ba3c8633261fc7fbbc96e758b0796f41addc40a1896`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811878d9e084fbf7c4d4c08d3f5d62c128d14cf147703b400436417f6a2e25ac`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 296.0 KB (296004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072405dc4b79db0e852b35ceb62ef6f2252c4322a430df8f44a50e9767e0c235`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.0-beta.1-windowsservercore` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:e3a8016c3c64a49897996ad69c0325e61752cdbc9ca844fa697f910bec8c98ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240771001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6e2b2b1ff8bf31f17438be13c2da7d529f76fcbe313e4eed06b9bc69f5d318`
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
# Wed, 13 Apr 2022 04:45:43 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:46:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:46:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:46:13 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:46:14 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:46:15 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:46:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:46:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:46:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:46:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:46:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:46:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:46:23 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:46:24 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:46:25 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:46:42 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:46:43 GMT
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
	-	`sha256:2e7d68c69939c53f016e8cf0d51d57a2b78dfcc512d66e66d6d2b4cb5a7f57b8`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f3727ab2382f41b18d95c8da347a7c755809b2191bf9f6a2fa46c171515824`  
		Last Modified: Wed, 13 Apr 2022 04:50:48 GMT  
		Size: 12.8 MB (12806637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dbb4d1a1e66edfd4b8227a146c73da1c1a5b984b7a709077d3df2b4619ed36`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25797b5f8af5b9846b486d46533da312930f863dca5d535061c13ac714cd8ec3`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccad74ccb9c577bc14a32134581b3f7d84f337fff019f4731b2a5f0c2c4b3f3`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c417f50c24094ea52e14331102360f4b3dd1b9f45719d1958f213f7ba645a5`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8fe45f94b2a2a75ff87a852e62b4fa9d18e5957365a0f3bfef85ee6da438f`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385801886c7f0293ab1b4b73193694ba1894a073b2ca5bf6735ba6ab16e34bc8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7d3e8a14bd7be12c7cbe40179fe5629f9446304feaadd2ab05fd465a0d3fd8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b92f30c475135a743a6752551f98a419b50f1ac541986c70339f36893f594f`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e80373ab79d4bd62bdd7971eb48f57334a2ce9ebd003647793e8a42025a7da8`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894294ebbe0380c696560955ca8e7b4007a9755305d872a7a08d2826f22ae734`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f6cd0e22f9513b18449e31ca425f5df0953cfb3e871179d34fd0fda91f728`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd68b9283a3e645eb13d6bf37b082a6405d6206ec33a1d9b8d57517c1d7dad23`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ec800f2a4638585b430b77da5a02fe8e5d739ae72a39869b2245eb7a8d8c6`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1671c65a57df30824e5058cf7fd6ac03442647e39234294e645cfd8f47c4a959`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c7e95b436b0a98f22b75bd760de1d59cef1cd2ecc16bd210204594698f727d`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cffba02c62a0ebbe70a3c5df4dacaa4054a9fcecc3b0c0a9d53896c6095e01e`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 346.0 KB (345957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2062b0d139ab02b47e030fb1a8980c3f3f86925f74de2fca500b7bc1f226a357`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:d8ed2af1d031d90876112d4136edc9dc1f8411861f37451ee7f85a6486187d68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2803; amd64

### `caddy:2.5.0-beta.1-windowsservercore-1809` - windows version 10.0.17763.2803; amd64

```console
$ docker pull caddy@sha256:6e626bf72e437a353d6d01d85f56a7ab74163cd1f9ca5132b70cc81b0ac95091
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2729197641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db2933cead23078da080b488af18ccea0fa4fcfe7157e8c7ed24eb9100f40e87`
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
# Wed, 13 Apr 2022 04:42:38 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:43:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:43:47 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:43:47 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:43:48 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:43:49 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:43:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:43:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:43:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:43:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:43:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:43:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:43:57 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:43:58 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:43:59 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:44:58 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:44:59 GMT
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
	-	`sha256:6f22b56b6abc68d2c947d2a5b077ed0ed9d7b9b281a92de72c0b337a88f7f52b`  
		Last Modified: Wed, 13 Apr 2022 04:50:29 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c010d9d46a653c0e43534061f409f08fc8276e27bf12dc32f301d0522851c72c`  
		Last Modified: Wed, 13 Apr 2022 04:50:32 GMT  
		Size: 12.6 MB (12577776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a0d3443230920064e9a4ad603b313c3c112274675ee2d708845c31b01dff9`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8ec8f791c42c04c3ef9e9f63a6b263171412c7e653edbfa0da0ec5e302bbd`  
		Last Modified: Wed, 13 Apr 2022 04:50:28 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d680fb76d896678fdd8db202fd05ccef68bc5dac499f1bb879a7afb9187fba`  
		Last Modified: Wed, 13 Apr 2022 04:50:27 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63775f08de58cfb563826ceb049f60eefecc09543520658d8c477b46ea054366`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d1ebc23d80d71f3f4c63af582cd73aec506328e3161ad08e6e22c3f3b1c631`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3070fa2a1cb5b58c6fc3d98dcf6dfe4190d619f757eaa321ae732ce5bdcb23`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cfe04dbc46bdb60c88f0aef2f22d16ddca431bbcfcbe8f9e54484a919e63ed`  
		Last Modified: Wed, 13 Apr 2022 04:50:26 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:612434bf8a03dd5fd2c666445bcf8e738df97316a3cfbf971751f10dada6e630`  
		Last Modified: Wed, 13 Apr 2022 04:50:25 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892e35d6a0cb734d147c4857708dd0da7717e8d3313f67b4243d3a1cc88ed3d`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4271146ce30c8ec1371049216f34f5c896cad13bd8c2d125dfb307d68c20ba2`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85bb125793433dd4c894875a1e1df0c00563c6773d50227c6887bcee5ab962d0`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d551fc39269de6a08e0405be92b691b0a0c5e1add58f6e8cb1d1aa745845bb5`  
		Last Modified: Wed, 13 Apr 2022 04:50:24 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd140311bf4ea4dda888642ca6d59e45279eca51b08fe5537dde2aa55b706ba`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14735299e19c40b09e06312a6309062c1984f1ba31f31392632fb498712e4978`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4384b686208549fdef850ba3c8633261fc7fbbc96e758b0796f41addc40a1896`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:811878d9e084fbf7c4d4c08d3f5d62c128d14cf147703b400436417f6a2e25ac`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 296.0 KB (296004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072405dc4b79db0e852b35ceb62ef6f2252c4322a430df8f44a50e9767e0c235`  
		Last Modified: Wed, 13 Apr 2022 04:50:22 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.0-beta.1-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:e7d11a1cc75c975ab2b66191eae9a26e01dd791235a103294bd614ef0703fd09
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `caddy:2.5.0-beta.1-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull caddy@sha256:e3a8016c3c64a49897996ad69c0325e61752cdbc9ca844fa697f910bec8c98ea
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2240771001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e6e2b2b1ff8bf31f17438be13c2da7d529f76fcbe313e4eed06b9bc69f5d318`
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
# Wed, 13 Apr 2022 04:45:43 GMT
ENV CADDY_VERSION=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.0-beta.1/caddy_2.5.0-beta.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d3823cb9ec107805c996e0de561c460a8d865698362c6ba842a69503af693d8f7db8ac418abffc4b7110a273d0b8be50168f8a5bcc0dc4da1e81fd1a4271f9d2')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 13 Apr 2022 04:46:11 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 13 Apr 2022 04:46:12 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 13 Apr 2022 04:46:13 GMT
VOLUME [c:/config]
# Wed, 13 Apr 2022 04:46:14 GMT
VOLUME [c:/data]
# Wed, 13 Apr 2022 04:46:15 GMT
LABEL org.opencontainers.image.version=v2.5.0-beta.1
# Wed, 13 Apr 2022 04:46:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 13 Apr 2022 04:46:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 13 Apr 2022 04:46:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 13 Apr 2022 04:46:19 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 13 Apr 2022 04:46:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 13 Apr 2022 04:46:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 13 Apr 2022 04:46:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 13 Apr 2022 04:46:23 GMT
EXPOSE 80
# Wed, 13 Apr 2022 04:46:24 GMT
EXPOSE 443
# Wed, 13 Apr 2022 04:46:25 GMT
EXPOSE 2019
# Wed, 13 Apr 2022 04:46:42 GMT
RUN caddy version
# Wed, 13 Apr 2022 04:46:43 GMT
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
	-	`sha256:2e7d68c69939c53f016e8cf0d51d57a2b78dfcc512d66e66d6d2b4cb5a7f57b8`  
		Last Modified: Wed, 13 Apr 2022 04:50:46 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2f3727ab2382f41b18d95c8da347a7c755809b2191bf9f6a2fa46c171515824`  
		Last Modified: Wed, 13 Apr 2022 04:50:48 GMT  
		Size: 12.8 MB (12806637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6dbb4d1a1e66edfd4b8227a146c73da1c1a5b984b7a709077d3df2b4619ed36`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25797b5f8af5b9846b486d46533da312930f863dca5d535061c13ac714cd8ec3`  
		Last Modified: Wed, 13 Apr 2022 04:50:45 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccad74ccb9c577bc14a32134581b3f7d84f337fff019f4731b2a5f0c2c4b3f3`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c417f50c24094ea52e14331102360f4b3dd1b9f45719d1958f213f7ba645a5`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8fe45f94b2a2a75ff87a852e62b4fa9d18e5957365a0f3bfef85ee6da438f`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:385801886c7f0293ab1b4b73193694ba1894a073b2ca5bf6735ba6ab16e34bc8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7d3e8a14bd7be12c7cbe40179fe5629f9446304feaadd2ab05fd465a0d3fd8`  
		Last Modified: Wed, 13 Apr 2022 04:50:43 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0b92f30c475135a743a6752551f98a419b50f1ac541986c70339f36893f594f`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e80373ab79d4bd62bdd7971eb48f57334a2ce9ebd003647793e8a42025a7da8`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894294ebbe0380c696560955ca8e7b4007a9755305d872a7a08d2826f22ae734`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e3f6cd0e22f9513b18449e31ca425f5df0953cfb3e871179d34fd0fda91f728`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd68b9283a3e645eb13d6bf37b082a6405d6206ec33a1d9b8d57517c1d7dad23`  
		Last Modified: Wed, 13 Apr 2022 04:50:41 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:460ec800f2a4638585b430b77da5a02fe8e5d739ae72a39869b2245eb7a8d8c6`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1671c65a57df30824e5058cf7fd6ac03442647e39234294e645cfd8f47c4a959`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c7e95b436b0a98f22b75bd760de1d59cef1cd2ecc16bd210204594698f727d`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cffba02c62a0ebbe70a3c5df4dacaa4054a9fcecc3b0c0a9d53896c6095e01e`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 346.0 KB (345957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2062b0d139ab02b47e030fb1a8980c3f3f86925f74de2fca500b7bc1f226a357`  
		Last Modified: Wed, 13 Apr 2022 04:50:39 GMT  
		Size: 1.4 KB (1420 bytes)  
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
$ docker pull caddy@sha256:14036c05891d952e4fb956693c2c63e50408107ad7507f524cd0ba883f1bb6b5
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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
$ docker pull caddy@sha256:e53c62d8939d3f0bb4c1ed28923d80f7e07dc3912b5a39d0476db918358cfa1f
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
$ docker pull caddy@sha256:f067c336bf9a0f6755735e5dbd07fdbce24f00d4ded39ae414599dd0707f5909
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114678400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6e18d0d8561f2864f5ae2184d369b7ed78f855c8098e12b18e3e66e9ed1d702`
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
# Tue, 05 Apr 2022 09:28:26 GMT
ENV GOLANG_VERSION=1.17.8
# Tue, 05 Apr 2022 09:31:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.17.8.src.tar.gz'; 		sha256='2effcd898140da79a061f3784ca4f8d8b13d811fb2abe9dad2404442dabbdf7a'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 05 Apr 2022 09:31:38 GMT
ENV GOPATH=/go
# Tue, 05 Apr 2022 09:31:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 09:31:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 05 Apr 2022 09:31:40 GMT
WORKDIR /go
# Wed, 06 Apr 2022 02:23:29 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 06 Apr 2022 02:23:29 GMT
ENV XCADDY_VERSION=v0.2.1
# Wed, 06 Apr 2022 02:23:30 GMT
ENV CADDY_VERSION=v2.4.6
# Wed, 06 Apr 2022 02:23:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 06 Apr 2022 02:23:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='30621f45934c6450dcf6ca790f2763a334ce58048a50e6d2b552a145da6cc0b79e454724d9953483794119c1b90555a8657e6311940cb37dd21c193e22459252' ;; 		armhf)   binArch='armv6'; checksum='5d1265a07be13aa9f2c9d8ad9a75d5658bca1dfc66c2b1b100b517edf4ac7a1fe18494c7b01b3856102e1cfc912912d049393accd8b1ef22f73bfc22bb27daec' ;; 		armv7)   binArch='armv7'; checksum='04e1b4c14def100db4c2da0c08d2bd48f1e965a6250763659a5e435d2815559483f7ce533e36cca9a15709508deab133972b19ff87a76f15ea01876a62e49edf' ;; 		aarch64) binArch='arm64'; checksum='e4cabca39b61c6a7956b828e9b1e1c39e802b65a1c1e3ce44d93bcffaafce6625884315815051f08209deb53a294101bf9c60ffbf000ac8ce2ba38a13e8e2287' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='ff1cc638ee18ce3ef36097547db9cdc3ff27f8ce46d8df50273663655ccea909a8396a01b4a144d57ad7e896ec6aef052c31f516c2a9c7e08d04a27228cf1c42' ;; 		s390x)   binArch='s390x'; checksum='335a7436927378508e0d55b74898b8d36f73f7a8ceaaa038c0ac054ab79c96b77acb642fb7881a07358b161e6e54efb8db0eacd0bd10f8f151698de517bffa0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.2.1/xcaddy_0.2.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Wed, 06 Apr 2022 02:23:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Wed, 06 Apr 2022 02:23:33 GMT
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
	-	`sha256:ce1c19e6ea71a7140e1f92aaf1ca20998b7875298f5f0aecdad1849acea539e9`  
		Last Modified: Tue, 05 Apr 2022 09:43:01 GMT  
		Size: 104.9 MB (104853355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d18ca61f70738e42fc01d4076606b8ef68be3c58058c1922e2b44987e87a15`  
		Last Modified: Tue, 05 Apr 2022 09:41:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d951a4c4c0e205bd2d3656382822e0ad97c4ee98c7cc185614d9363d5b7b18df`  
		Last Modified: Wed, 06 Apr 2022 02:25:20 GMT  
		Size: 6.0 MB (5952176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14b38ba848bdb94dd4baa0c3e1ed84c6c0f039346dbd2904d5e257b874558a07`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 1.2 MB (1176713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426c201900d8690c727d61a628a8540811cafc07c1ed656aeb066b7745707c7b`  
		Last Modified: Wed, 06 Apr 2022 02:25:18 GMT  
		Size: 406.0 B  
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
