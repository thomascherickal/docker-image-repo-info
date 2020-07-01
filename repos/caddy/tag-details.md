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
$ docker pull caddy@sha256:4109bb1ba7965c1db17e985891344881c9566fe7832ff593da7ddfc98a16c2fe
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
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:4109bb1ba7965c1db17e985891344881c9566fe7832ff593da7ddfc98a16c2fe
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

### `caddy:2.1.1` - linux; amd64

```console
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-alpine`

```console
$ docker pull caddy@sha256:707e960e783141b786754199242c2aa10046712e7b2697aa3bc030492c50de2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder`

```console
$ docker pull caddy@sha256:aaccc5619af0303dd34155904cd0a59126d806494344a82b50ae40b75474d221
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.1.1-builder` - linux; amd64

```console
$ docker pull caddy@sha256:4f017fc1ac4111aef9f4cdc6b9c3823a8dc602147424e1d64c5f2401e11464f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330843445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae42fca94e0c95c78cd48a8f3406f0d7ac7109215f0f42ac1c985fafb5fef8b`
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
# Wed, 01 Jul 2020 00:19:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:46 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:19:46 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 00:20:00 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 00:20:01 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 00:20:01 GMT
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
	-	`sha256:c5739bbf0a0f9e7d0662bda893cb8cf60bb3a2e05f18a9877ffc9ed68bffedc2`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 3.1 MB (3099624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9fc833b22a6c6a92b57020c0561451a6a48c84fa6acbcafe73d69c4b14492`  
		Last Modified: Wed, 01 Jul 2020 00:20:44 GMT  
		Size: 184.2 MB (184231858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e45c1d9abc61951202274f83b4702c140365c11a3839dedf2ddff747950e79`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b2d315c798f5c7da86068461d3ea55fdfa1d3d36f6fa461ef788610041848`  
		Last Modified: Wed, 01 Jul 2020 00:20:22 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e22e313c0b989a14734b7d6a870cbb161d3bbce596d0464c1a4a30e29eed42a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326364241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89d3a9be9f9b9317c9fb9f9595f14842ed72bee937e42e2c5dc9736a0184f7`
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
# Tue, 30 Jun 2020 23:49:51 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:54 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:49:55 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:50:38 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:50:43 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:50:44 GMT
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
	-	`sha256:87454bdd0b68cb419479596ea418f39e543899d1bcf4a9b8438e4a0af915d659`  
		Last Modified: Tue, 30 Jun 2020 23:51:17 GMT  
		Size: 3.1 MB (3099715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8248605a05ee8d00c6a13d2b522c366652ff839231107c73f8e02086e2ef5b1c`  
		Last Modified: Tue, 30 Jun 2020 23:52:04 GMT  
		Size: 184.2 MB (184239271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff94bab35f82fddff7da755a0e8be00e7eb4d5e609dd18f7f11973bc7a4b08`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46449ce8dce15ddfd740cdda07cd834fbea8324e44a8dc86e9418d8930d8fbe5`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ea13ba0955867cd8791ecf56011867e07366da796332f3fa0067eb6bcff7ab1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325014324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccf5f7db893915e1f867d483712da1b4b6fb3cc5f737a029edb8d67b500714f`
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
# Tue, 30 Jun 2020 23:58:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:58:24 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:58:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:59:13 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:59:19 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:59:20 GMT
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
	-	`sha256:bff70e09616486f12dbaa23bf518b25b4319b9191a192b458fb1a54ce5de4d3b`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 3.1 MB (3097567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286df284eb60ab6779cc5d8f805e5ca5deecdc9b3cef6384bc1ff223e36c1d99`  
		Last Modified: Wed, 01 Jul 2020 00:00:45 GMT  
		Size: 184.2 MB (184235432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4619955daf96563227c47cbcc91a0d932a40bf618feac706639545114e1548`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaf4511144a3e7894cdfd495c3544d22d4226fa3f0f11fad1cb8dc998875b21`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd14a703ad5a26ffa7de82fbf23106617876e6542e6cae4bb11cdfd7fecf0985
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325331656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226bb48667615278e4dee44611a6f3bc288af0cbf1f080226dcc308275141482`
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
# Tue, 30 Jun 2020 23:40:08 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:40:11 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:40:12 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:40:39 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:40:46 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:40:46 GMT
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
	-	`sha256:40cc98ebf8ade7d14e8ba21309fb3ec00ecd3f5c26bcde20da0a4404592a452d`  
		Last Modified: Tue, 30 Jun 2020 23:41:16 GMT  
		Size: 3.1 MB (3097543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896511aaf0a6d921f248b7e9c422cafcf89eeb3767cb1c3b8fb120b99d130177`  
		Last Modified: Tue, 30 Jun 2020 23:41:57 GMT  
		Size: 184.2 MB (184237073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bea5a4cbbd78d491a7e68e2416b08b338f44dc16391b392cfee8bc7402cdca0`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8478b518bb5c87d93de66aee41cd91abdf4ef7f6132fb047b5437d86ce0f020`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:396e07a9cdc415aec2af853cdfc546f68e3e3524b6b66a00fa510eda3cd47c6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.6 MB (324617612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc68a9a7841d30d5b52a374362b68a95a217f600eb5f0e7b002657682dbf81a2`
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
# Wed, 01 Jul 2020 00:54:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:55:18 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:55:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 01:00:44 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 01:00:50 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 01:00:54 GMT
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
	-	`sha256:6576be449bd2776954e56f7254b1d88000e75ad86165473cf13427acc05615ca`  
		Last Modified: Wed, 01 Jul 2020 01:01:44 GMT  
		Size: 3.1 MB (3097500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9480caee021b774a13782504a3b88c52bcde123400ecce3b764df8cb7eb224`  
		Last Modified: Wed, 01 Jul 2020 01:02:12 GMT  
		Size: 184.2 MB (184244849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661dd2e4685659ab41e26790a0e6fe86056e887993933e3ebed22cea585ec903`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6938d2ac44364da5bcff7ab862c4620f5f24c30347f21b6fcd3900806923d7dc`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:abece892e9c1d34cf4e58818b6e955f1245042d7c9af17a76e5d4871d05b680f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330350401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c515a83c152d93961b4a06516fa3dfa07c586364f26f1032073d2f6a67cbb2b5`
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
# Tue, 30 Jun 2020 23:41:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:41:48 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:42:14 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:42:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:42:29 GMT
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
	-	`sha256:d4b8ff85b28f8ebc6d191d86a31b77fe5f1b972d7a27b84107f388dd9d7e94be`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 3.1 MB (3099677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64998b03655d547eb0910c16089828b9da3dcfc52fe9d4630cc9af3f0f2a15a9`  
		Last Modified: Tue, 30 Jun 2020 23:43:18 GMT  
		Size: 184.2 MB (184233221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41d0d57ba486d3311fcc98ee48f170ee2f22db1f24ac5e20a7fa11bb8a6c025`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4634fdf0713a3dbf80607ad3b2210af124d3c2295c1e642e9f1371cfe5777`  
		Last Modified: Tue, 30 Jun 2020 23:43:01 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:6bea7b35517a171929f356010eb1b9203f6e2425b23bf60eac0416f9ddb84833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6a5e85d8268fdf2dc72fc43dfb70a4a170c63e7c68f441fb87943a916142a752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be0404997cbeb408e6b8b3685912b7670868aed482bf81264f55e86cedf0d5b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:707e960e783141b786754199242c2aa10046712e7b2697aa3bc030492c50de2a
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
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:aaccc5619af0303dd34155904cd0a59126d806494344a82b50ae40b75474d221
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
$ docker pull caddy@sha256:4f017fc1ac4111aef9f4cdc6b9c3823a8dc602147424e1d64c5f2401e11464f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330843445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae42fca94e0c95c78cd48a8f3406f0d7ac7109215f0f42ac1c985fafb5fef8b`
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
# Wed, 01 Jul 2020 00:19:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:46 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:19:46 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 00:20:00 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 00:20:01 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 00:20:01 GMT
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
	-	`sha256:c5739bbf0a0f9e7d0662bda893cb8cf60bb3a2e05f18a9877ffc9ed68bffedc2`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 3.1 MB (3099624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9fc833b22a6c6a92b57020c0561451a6a48c84fa6acbcafe73d69c4b14492`  
		Last Modified: Wed, 01 Jul 2020 00:20:44 GMT  
		Size: 184.2 MB (184231858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e45c1d9abc61951202274f83b4702c140365c11a3839dedf2ddff747950e79`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b2d315c798f5c7da86068461d3ea55fdfa1d3d36f6fa461ef788610041848`  
		Last Modified: Wed, 01 Jul 2020 00:20:22 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e22e313c0b989a14734b7d6a870cbb161d3bbce596d0464c1a4a30e29eed42a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326364241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89d3a9be9f9b9317c9fb9f9595f14842ed72bee937e42e2c5dc9736a0184f7`
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
# Tue, 30 Jun 2020 23:49:51 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:54 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:49:55 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:50:38 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:50:43 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:50:44 GMT
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
	-	`sha256:87454bdd0b68cb419479596ea418f39e543899d1bcf4a9b8438e4a0af915d659`  
		Last Modified: Tue, 30 Jun 2020 23:51:17 GMT  
		Size: 3.1 MB (3099715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8248605a05ee8d00c6a13d2b522c366652ff839231107c73f8e02086e2ef5b1c`  
		Last Modified: Tue, 30 Jun 2020 23:52:04 GMT  
		Size: 184.2 MB (184239271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff94bab35f82fddff7da755a0e8be00e7eb4d5e609dd18f7f11973bc7a4b08`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46449ce8dce15ddfd740cdda07cd834fbea8324e44a8dc86e9418d8930d8fbe5`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ea13ba0955867cd8791ecf56011867e07366da796332f3fa0067eb6bcff7ab1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325014324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccf5f7db893915e1f867d483712da1b4b6fb3cc5f737a029edb8d67b500714f`
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
# Tue, 30 Jun 2020 23:58:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:58:24 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:58:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:59:13 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:59:19 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:59:20 GMT
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
	-	`sha256:bff70e09616486f12dbaa23bf518b25b4319b9191a192b458fb1a54ce5de4d3b`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 3.1 MB (3097567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286df284eb60ab6779cc5d8f805e5ca5deecdc9b3cef6384bc1ff223e36c1d99`  
		Last Modified: Wed, 01 Jul 2020 00:00:45 GMT  
		Size: 184.2 MB (184235432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4619955daf96563227c47cbcc91a0d932a40bf618feac706639545114e1548`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaf4511144a3e7894cdfd495c3544d22d4226fa3f0f11fad1cb8dc998875b21`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd14a703ad5a26ffa7de82fbf23106617876e6542e6cae4bb11cdfd7fecf0985
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325331656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226bb48667615278e4dee44611a6f3bc288af0cbf1f080226dcc308275141482`
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
# Tue, 30 Jun 2020 23:40:08 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:40:11 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:40:12 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:40:39 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:40:46 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:40:46 GMT
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
	-	`sha256:40cc98ebf8ade7d14e8ba21309fb3ec00ecd3f5c26bcde20da0a4404592a452d`  
		Last Modified: Tue, 30 Jun 2020 23:41:16 GMT  
		Size: 3.1 MB (3097543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896511aaf0a6d921f248b7e9c422cafcf89eeb3767cb1c3b8fb120b99d130177`  
		Last Modified: Tue, 30 Jun 2020 23:41:57 GMT  
		Size: 184.2 MB (184237073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bea5a4cbbd78d491a7e68e2416b08b338f44dc16391b392cfee8bc7402cdca0`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8478b518bb5c87d93de66aee41cd91abdf4ef7f6132fb047b5437d86ce0f020`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:396e07a9cdc415aec2af853cdfc546f68e3e3524b6b66a00fa510eda3cd47c6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.6 MB (324617612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc68a9a7841d30d5b52a374362b68a95a217f600eb5f0e7b002657682dbf81a2`
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
# Wed, 01 Jul 2020 00:54:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:55:18 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:55:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 01:00:44 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 01:00:50 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 01:00:54 GMT
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
	-	`sha256:6576be449bd2776954e56f7254b1d88000e75ad86165473cf13427acc05615ca`  
		Last Modified: Wed, 01 Jul 2020 01:01:44 GMT  
		Size: 3.1 MB (3097500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9480caee021b774a13782504a3b88c52bcde123400ecce3b764df8cb7eb224`  
		Last Modified: Wed, 01 Jul 2020 01:02:12 GMT  
		Size: 184.2 MB (184244849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661dd2e4685659ab41e26790a0e6fe86056e887993933e3ebed22cea585ec903`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6938d2ac44364da5bcff7ab862c4620f5f24c30347f21b6fcd3900806923d7dc`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:abece892e9c1d34cf4e58818b6e955f1245042d7c9af17a76e5d4871d05b680f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330350401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c515a83c152d93961b4a06516fa3dfa07c586364f26f1032073d2f6a67cbb2b5`
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
# Tue, 30 Jun 2020 23:41:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:41:48 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:42:14 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:42:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:42:29 GMT
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
	-	`sha256:d4b8ff85b28f8ebc6d191d86a31b77fe5f1b972d7a27b84107f388dd9d7e94be`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 3.1 MB (3099677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64998b03655d547eb0910c16089828b9da3dcfc52fe9d4630cc9af3f0f2a15a9`  
		Last Modified: Tue, 30 Jun 2020 23:43:18 GMT  
		Size: 184.2 MB (184233221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41d0d57ba486d3311fcc98ee48f170ee2f22db1f24ac5e20a7fa11bb8a6c025`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4634fdf0713a3dbf80607ad3b2210af124d3c2295c1e642e9f1371cfe5777`  
		Last Modified: Tue, 30 Jun 2020 23:43:01 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:6bea7b35517a171929f356010eb1b9203f6e2425b23bf60eac0416f9ddb84833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6a5e85d8268fdf2dc72fc43dfb70a4a170c63e7c68f441fb87943a916142a752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be0404997cbeb408e6b8b3685912b7670868aed482bf81264f55e86cedf0d5b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:707e960e783141b786754199242c2aa10046712e7b2697aa3bc030492c50de2a
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
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:aaccc5619af0303dd34155904cd0a59126d806494344a82b50ae40b75474d221
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
$ docker pull caddy@sha256:4f017fc1ac4111aef9f4cdc6b9c3823a8dc602147424e1d64c5f2401e11464f6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.8 MB (330843445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fae42fca94e0c95c78cd48a8f3406f0d7ac7109215f0f42ac1c985fafb5fef8b`
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
# Wed, 01 Jul 2020 00:19:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:46 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:19:46 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 00:20:00 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 00:20:01 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 00:20:01 GMT
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
	-	`sha256:c5739bbf0a0f9e7d0662bda893cb8cf60bb3a2e05f18a9877ffc9ed68bffedc2`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 3.1 MB (3099624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9fc833b22a6c6a92b57020c0561451a6a48c84fa6acbcafe73d69c4b14492`  
		Last Modified: Wed, 01 Jul 2020 00:20:44 GMT  
		Size: 184.2 MB (184231858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e45c1d9abc61951202274f83b4702c140365c11a3839dedf2ddff747950e79`  
		Last Modified: Wed, 01 Jul 2020 00:20:23 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b2d315c798f5c7da86068461d3ea55fdfa1d3d36f6fa461ef788610041848`  
		Last Modified: Wed, 01 Jul 2020 00:20:22 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:e22e313c0b989a14734b7d6a870cbb161d3bbce596d0464c1a4a30e29eed42a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326364241 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c89d3a9be9f9b9317c9fb9f9595f14842ed72bee937e42e2c5dc9736a0184f7`
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
# Tue, 30 Jun 2020 23:49:51 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:54 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:49:55 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:50:38 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:50:43 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:50:44 GMT
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
	-	`sha256:87454bdd0b68cb419479596ea418f39e543899d1bcf4a9b8438e4a0af915d659`  
		Last Modified: Tue, 30 Jun 2020 23:51:17 GMT  
		Size: 3.1 MB (3099715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8248605a05ee8d00c6a13d2b522c366652ff839231107c73f8e02086e2ef5b1c`  
		Last Modified: Tue, 30 Jun 2020 23:52:04 GMT  
		Size: 184.2 MB (184239271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff94bab35f82fddff7da755a0e8be00e7eb4d5e609dd18f7f11973bc7a4b08`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46449ce8dce15ddfd740cdda07cd834fbea8324e44a8dc86e9418d8930d8fbe5`  
		Last Modified: Tue, 30 Jun 2020 23:51:16 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:0ea13ba0955867cd8791ecf56011867e07366da796332f3fa0067eb6bcff7ab1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.0 MB (325014324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccf5f7db893915e1f867d483712da1b4b6fb3cc5f737a029edb8d67b500714f`
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
# Tue, 30 Jun 2020 23:58:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:58:24 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:58:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:59:13 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:59:19 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:59:20 GMT
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
	-	`sha256:bff70e09616486f12dbaa23bf518b25b4319b9191a192b458fb1a54ce5de4d3b`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 3.1 MB (3097567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286df284eb60ab6779cc5d8f805e5ca5deecdc9b3cef6384bc1ff223e36c1d99`  
		Last Modified: Wed, 01 Jul 2020 00:00:45 GMT  
		Size: 184.2 MB (184235432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f4619955daf96563227c47cbcc91a0d932a40bf618feac706639545114e1548`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efaf4511144a3e7894cdfd495c3544d22d4226fa3f0f11fad1cb8dc998875b21`  
		Last Modified: Tue, 30 Jun 2020 23:59:55 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:dd14a703ad5a26ffa7de82fbf23106617876e6542e6cae4bb11cdfd7fecf0985
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325331656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:226bb48667615278e4dee44611a6f3bc288af0cbf1f080226dcc308275141482`
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
# Tue, 30 Jun 2020 23:40:08 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:40:11 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:40:12 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:40:39 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:40:46 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:40:46 GMT
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
	-	`sha256:40cc98ebf8ade7d14e8ba21309fb3ec00ecd3f5c26bcde20da0a4404592a452d`  
		Last Modified: Tue, 30 Jun 2020 23:41:16 GMT  
		Size: 3.1 MB (3097543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:896511aaf0a6d921f248b7e9c422cafcf89eeb3767cb1c3b8fb120b99d130177`  
		Last Modified: Tue, 30 Jun 2020 23:41:57 GMT  
		Size: 184.2 MB (184237073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bea5a4cbbd78d491a7e68e2416b08b338f44dc16391b392cfee8bc7402cdca0`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8478b518bb5c87d93de66aee41cd91abdf4ef7f6132fb047b5437d86ce0f020`  
		Last Modified: Tue, 30 Jun 2020 23:41:15 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:396e07a9cdc415aec2af853cdfc546f68e3e3524b6b66a00fa510eda3cd47c6f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.6 MB (324617612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc68a9a7841d30d5b52a374362b68a95a217f600eb5f0e7b002657682dbf81a2`
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
# Wed, 01 Jul 2020 00:54:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:55:18 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 01 Jul 2020 00:55:25 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 01 Jul 2020 01:00:44 GMT
RUN go get -d ./...
# Wed, 01 Jul 2020 01:00:50 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Wed, 01 Jul 2020 01:00:54 GMT
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
	-	`sha256:6576be449bd2776954e56f7254b1d88000e75ad86165473cf13427acc05615ca`  
		Last Modified: Wed, 01 Jul 2020 01:01:44 GMT  
		Size: 3.1 MB (3097500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe9480caee021b774a13782504a3b88c52bcde123400ecce3b764df8cb7eb224`  
		Last Modified: Wed, 01 Jul 2020 01:02:12 GMT  
		Size: 184.2 MB (184244849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661dd2e4685659ab41e26790a0e6fe86056e887993933e3ebed22cea585ec903`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6938d2ac44364da5bcff7ab862c4620f5f24c30347f21b6fcd3900806923d7dc`  
		Last Modified: Wed, 01 Jul 2020 01:01:43 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:abece892e9c1d34cf4e58818b6e955f1245042d7c9af17a76e5d4871d05b680f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330350401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c515a83c152d93961b4a06516fa3dfa07c586364f26f1032073d2f6a67cbb2b5`
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
# Tue, 30 Jun 2020 23:41:45 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:47 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 30 Jun 2020 23:41:48 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 30 Jun 2020 23:42:14 GMT
RUN go get -d ./...
# Tue, 30 Jun 2020 23:42:28 GMT
COPY file:83b813b69aee8796ce6cdf324efd1e9890d70da3ae40d917ee2f320c487134c6 in /usr/bin/caddy-builder 
# Tue, 30 Jun 2020 23:42:29 GMT
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
	-	`sha256:d4b8ff85b28f8ebc6d191d86a31b77fe5f1b972d7a27b84107f388dd9d7e94be`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 3.1 MB (3099677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64998b03655d547eb0910c16089828b9da3dcfc52fe9d4630cc9af3f0f2a15a9`  
		Last Modified: Tue, 30 Jun 2020 23:43:18 GMT  
		Size: 184.2 MB (184233221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41d0d57ba486d3311fcc98ee48f170ee2f22db1f24ac5e20a7fa11bb8a6c025`  
		Last Modified: Tue, 30 Jun 2020 23:42:56 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa4634fdf0713a3dbf80607ad3b2210af124d3c2295c1e642e9f1371cfe5777`  
		Last Modified: Tue, 30 Jun 2020 23:43:01 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:4109bb1ba7965c1db17e985891344881c9566fe7832ff593da7ddfc98a16c2fe
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
$ docker pull caddy@sha256:9ce811ab3540971fab00748e5d9a6bc7a91518fc9848367c907e32fda8d01411
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16160777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a12b5c957bab94f57aadfd9e655d414ab69443495f22ef430152181ab0aede`
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
# Wed, 01 Jul 2020 00:19:34 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:19:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:19:37 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:19:37 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:19:37 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:19:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:19:39 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:19:39 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:19:40 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:19:40 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:19:40 GMT
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
	-	`sha256:57d6f0d7c084024816c9d62c8cf79558a18c5df4cdcc951484a9e0ca63dd0b72`  
		Last Modified: Wed, 01 Jul 2020 00:20:17 GMT  
		Size: 13.1 MB (13057334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639b35073727cad03304869adcd7b9118cd8039707d055f5b37992f7188076d3`  
		Last Modified: Wed, 01 Jul 2020 00:20:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c8dd4b191727d7eccb50cdf3f3d26fe19abbd23be153dfd53a11f01059002928
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.3 MB (15324343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352f7aeefb2f9e7015bf833505ff90d75dc751bfa7d202255900787d9c1a6e1a`
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
# Tue, 30 Jun 2020 23:49:25 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:49:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:49:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:49:32 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:49:33 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:49:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:49:34 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:49:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:49:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:49:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:49:38 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:49:39 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:49:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:49:41 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:49:42 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:49:43 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:49:43 GMT
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
	-	`sha256:82ed8e0a01609838fd9b844360403b0c62d26ca345d311c0e12ce9b3b7598f38`  
		Last Modified: Tue, 30 Jun 2020 23:51:10 GMT  
		Size: 12.4 MB (12414918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697e38da42d8f15b4dd54f63870d7e806d1eb7fc0fa15968afda08c82ebb567d`  
		Last Modified: Tue, 30 Jun 2020 23:51:09 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:251cd735b768dece1a258fe61d2f5f17489920c820d5ed42c431bf03df06c62b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.1 MB (15108010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5b113527fd3cc583349e001c913567cb5ae6f17df91d84b587c597a69e63574`
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
# Tue, 30 Jun 2020 23:57:45 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:57:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:57:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:57:58 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:57:59 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:58:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:58:01 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:58:03 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:58:05 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:58:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:58:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:58:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:58:09 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:58:10 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:58:11 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:58:12 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:58:13 GMT
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
	-	`sha256:2650c88e8e905db99ee64cc19f474dc3c7a32c737e05c403dcda6d96cbee69c4`  
		Last Modified: Tue, 30 Jun 2020 23:59:49 GMT  
		Size: 12.4 MB (12396011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8987db1ddf93e7c11e4c142ecfc8724b54131c3a5bf498a315d3c3dc6846990`  
		Last Modified: Tue, 30 Jun 2020 23:59:46 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:788931ce2b8e71b550976686f4085c0d4916bdbcc762f9db67d6f0036a109897
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.0 MB (15027460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b8f97e703682d7f83ea2a0146297c030599f59b72b006da9f851c8594777f`
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
# Tue, 30 Jun 2020 23:39:44 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:39:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:39:50 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:39:51 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:39:51 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:39:52 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:39:53 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:39:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:39:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:39:56 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:39:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:39:58 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:39:59 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:40:00 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:40:00 GMT
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
	-	`sha256:cbb12521bcb6d56dcfc220f0b20353a7aa329d702f5feb52f41bcf589de54695`  
		Last Modified: Tue, 30 Jun 2020 23:41:07 GMT  
		Size: 12.0 MB (12013102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599000c030713113e35f054497b6ea20d7cfe46540c547c904d1cb29e5ab5e09`  
		Last Modified: Tue, 30 Jun 2020 23:41:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:eda12afcf0918e61a08bdd958c9c41e599ef640367a8a50b21c7208d3864b9ed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.9 MB (14899035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2fd2d02dd7c74b824afe02694093d9ad27a7fe4da1f70dc8f499d714c0de004`
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
# Wed, 01 Jul 2020 00:52:33 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:52:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 01 Jul 2020 00:53:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 01 Jul 2020 00:53:10 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 01 Jul 2020 00:53:13 GMT
ENV XDG_DATA_HOME=/data
# Wed, 01 Jul 2020 00:53:18 GMT
VOLUME [/config]
# Wed, 01 Jul 2020 00:53:24 GMT
VOLUME [/data]
# Wed, 01 Jul 2020 00:53:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:53:34 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:53:44 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:53:53 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:53:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:54:05 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:54:11 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:54:14 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:54:20 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:54:29 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:54:38 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:54:41 GMT
WORKDIR /srv
# Wed, 01 Jul 2020 00:54:46 GMT
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
	-	`sha256:4370c1e51003a37803d04248bb3fbf1f56ca3809ab021a4e661b6d39fb8ef21f`  
		Last Modified: Wed, 01 Jul 2020 01:01:31 GMT  
		Size: 11.8 MB (11785466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2acf474ff4d447e0ee036263e810f271f045341957b949e742c4299ff7e8199a`  
		Last Modified: Wed, 01 Jul 2020 01:01:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:c15a47ccc69b6ea56daff5a268d5e93e40faf8ca0124f19c065e301e8ad4bedd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15709487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1e80a8389cb6f5ffcd0f2092c3c3898d44aa2d3035a3c7482e315a32626622d`
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
# Tue, 30 Jun 2020 23:41:28 GMT
ENV CADDY_VERSION=v2.1.1
# Tue, 30 Jun 2020 23:41:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='41f2442c52daf5a36d07af5024711072925997d8b5a7bd459994b000cfee1cb63d0c97d1b54b172c59b6b02a0f0eab285141a8cd3fc23cbca684f824c7b21b75' ;; 		armhf)   binArch='armv6'; checksum='91b69356155b4909feec8c4e5674a52d13c75b5c4bedfa3c7be2615a18cecbb58212de753d288ecd355502412d33bde9beed713055263636039ee4c47466ca90' ;; 		armv7)   binArch='armv7'; checksum='e45d8c8ac9fab83a26660531ef117dd0fbcaf81e442bb01f0d068afda6c507e692105e0c7f5fb86f227cf7693bff12b63647377e72571dc98c2dd0b6a7d76d81' ;; 		aarch64) binArch='arm64'; checksum='8d9d873e701ab2dfe6046c5f6a9bbd19dd2aef7e4c57640c897e70cc5d2775353f0c467779e2fba4c024c9de89d2b1d64c1b46568dda65e6f5a114f13b239c6d' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='30248cca16ec07e1e9aee0dabaaf0959f2f3622aafbdd9dac9135a4f2117ca3cc5b5bbfb8c94d45ea2c1abf61840587885f2db7fec420cd00918819cd39bfc92' ;; 		s390x)   binArch='s390x'; checksum='f4e16ad4f03f13cbe463efb8577d99f22a30161916cde10f5a0c838f7c57022b572b9a18d25fb20925aef4a5366537948ffdd4a191b3d5205ab9ab980406ca4b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 30 Jun 2020 23:41:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 30 Jun 2020 23:41:33 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 30 Jun 2020 23:41:34 GMT
ENV XDG_DATA_HOME=/data
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/config]
# Tue, 30 Jun 2020 23:41:34 GMT
VOLUME [/data]
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Tue, 30 Jun 2020 23:41:35 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 30 Jun 2020 23:41:36 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 30 Jun 2020 23:41:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 30 Jun 2020 23:41:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 80
# Tue, 30 Jun 2020 23:41:38 GMT
EXPOSE 443
# Tue, 30 Jun 2020 23:41:39 GMT
EXPOSE 2019
# Tue, 30 Jun 2020 23:41:39 GMT
WORKDIR /srv
# Tue, 30 Jun 2020 23:41:40 GMT
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
	-	`sha256:59a74ac154ef35abae9974398394ecc94fe54ad18af49231bc6a337fc43346c5`  
		Last Modified: Tue, 30 Jun 2020 23:42:46 GMT  
		Size: 12.8 MB (12836780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5673e745c5f3d1ac989f1a9cc90e301eb65e6dec0d3875d0480300738a959f32`  
		Last Modified: Tue, 30 Jun 2020 23:42:44 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:6bea7b35517a171929f356010eb1b9203f6e2425b23bf60eac0416f9ddb84833
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:6a5e85d8268fdf2dc72fc43dfb70a4a170c63e7c68f441fb87943a916142a752
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1282; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1282; amd64

```console
$ docker pull caddy@sha256:77457a1d020bd33050143d17846f94c0caa328868a22620c22792c842fa9847c
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2312351756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90fe8eb1d91b21db1e55c3cb01033e1ef8ac50675b44e322cfd952468ae3fb37`
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
# Wed, 01 Jul 2020 00:15:29 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:15:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:16:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:16:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:16:03 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:16:04 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:16:04 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:16:05 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:16:06 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:16:07 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:16:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:16:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:16:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:16:11 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:16:12 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:16:13 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:16:29 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:16:30 GMT
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
	-	`sha256:6bc338e95aacf0df61c8d7a8f6829ca9f7adacd3d48f2f08006bf6c260e6f6a1`  
		Last Modified: Wed, 01 Jul 2020 00:19:33 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e83e5ec896196d3a3b38f7d121d59d2b855f0dad39906b250a24b836c94b08c`  
		Last Modified: Wed, 01 Jul 2020 00:19:34 GMT  
		Size: 13.3 MB (13344221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91139d50f5068c10450d400b2a7f95fd20c7cb9dfafef759b664aa0e3994ac9f`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c88a225f30963de8211710e04403d1f5a0977c97667a2f73fe89a8fe8ed78aa`  
		Last Modified: Wed, 01 Jul 2020 00:19:31 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccd8b4dc035d4502f79bdc5040291ba7700285c35b2575cdbc6a948cbcbe816a`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aade01ab5b296bdffd61a3849c5c2feb03618880c5a257ea02496adf0615f26`  
		Last Modified: Wed, 01 Jul 2020 00:19:30 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dd47640bcab2ae58a8eb8b6b28b8babd8cd800966e426abef67c9c237fa756d`  
		Last Modified: Wed, 01 Jul 2020 00:19:29 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa16ffeedca2e162258cff0b1d2f84ea8f35088236dd08e957122949042f4b9b`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88aa8b5af14fa9a21fdf1d69de1f539fcbd9ce53dd714cafe2a3fb23506af45`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d5db36198ee72f508e31517e6883f316d91f95958a81dd9bc386f745282b467`  
		Last Modified: Wed, 01 Jul 2020 00:19:28 GMT  
		Size: 1.1 KB (1102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3daa6b70ac7530f10ab82868ce40ee01776676e25eb487fcc76c115d6af264`  
		Last Modified: Wed, 01 Jul 2020 00:19:27 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b566a496c2533383f4f0123fc7c110b861b4ee66bfe2399ba5b60dada395f78`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b678d312023c6e6bcc37e8fcd954ccbb28b373021cad45f3c2a1bbca7692ff`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:853e01c72e5605721fad676ecef92f48af0afc4a9261755036c45cb19294e50d`  
		Last Modified: Wed, 01 Jul 2020 00:19:26 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8965b8925adb333a05f00219d90ae6cf09de041cfaf8595360fae18080655e70`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227dbe25decc1868fbf806fee9b1b273af973a1ebbfe49e5d257cc986f4715a5`  
		Last Modified: Wed, 01 Jul 2020 00:19:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:258739e6b29b47678291ece5458686f3a59043b4d75cecae04bd82fff7b10e00`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf80ae83e0f501d308bec53bf5b048310f827038a13774104a0d551766b0c0cf`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 298.6 KB (298594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135756e2e12ff222ace60a5ca0c860b1047e6cb58196b7818b51a1f969272c2`  
		Last Modified: Wed, 01 Jul 2020 00:19:24 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:be0404997cbeb408e6b8b3685912b7670868aed482bf81264f55e86cedf0d5b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3750; amd64

```console
$ docker pull caddy@sha256:35faf7e24fb90b61a662f6dc0bb5907b51962e6f9db230ff97a9fffdf519d84f
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5758041528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c204aa0e66f6a68b3028da90168170b188478eec673c56f7a97bf35ad6e58a`
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
# Wed, 01 Jul 2020 00:16:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 01 Jul 2020 00:17:56 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 01 Jul 2020 00:17:58 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 01 Jul 2020 00:18:00 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 01 Jul 2020 00:18:01 GMT
VOLUME [c:/config]
# Wed, 01 Jul 2020 00:18:02 GMT
VOLUME [c:/data]
# Wed, 01 Jul 2020 00:18:03 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 01 Jul 2020 00:18:04 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 01 Jul 2020 00:18:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 01 Jul 2020 00:18:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 01 Jul 2020 00:18:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 01 Jul 2020 00:18:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 01 Jul 2020 00:18:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 01 Jul 2020 00:18:10 GMT
EXPOSE 80
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 443
# Wed, 01 Jul 2020 00:18:11 GMT
EXPOSE 2019
# Wed, 01 Jul 2020 00:18:53 GMT
RUN caddy version
# Wed, 01 Jul 2020 00:18:53 GMT
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
	-	`sha256:70815a4e602dcb92adf9e14c510bcf6daa720fb66605edb0b27add0b89bff54f`  
		Last Modified: Wed, 01 Jul 2020 00:19:57 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f44ce30c89d63dc99d1968700a55b80f0d99aad65ba89f4ee3ade2d381c3f4`  
		Last Modified: Wed, 01 Jul 2020 00:20:01 GMT  
		Size: 18.4 MB (18377062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17cf10e58e9a122e35be1735717c61c61cd1deadb0773235286ae62223a2e315`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6161a0fcceb4a26debf861062c6829b28f136d137f849005c69597c42417b3e`  
		Last Modified: Wed, 01 Jul 2020 00:19:56 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eb7f8a27aae00f64c6aa3145e6c337b93a385cc4b870f3b720a29b031a64914`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b36518163a26c3002588a267ddfc7160e6ab70b5379b5c313db0810d393f00`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b567a1e63379dfda7bae18e6795b77debd7fb5ab62d5ae2d10b79096becb381`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75eec6a21fc9b9a5f4c2c477a303711c5c1c32af96e7964d34093c46e2fdfdb2`  
		Last Modified: Wed, 01 Jul 2020 00:19:54 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b46643e395de1cd6d34af71ff25ceec8235661fd565ad75f778234e8dcfc5`  
		Last Modified: Wed, 01 Jul 2020 00:19:53 GMT  
		Size: 1.2 KB (1170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a0e022176d77fe5b17cc2164652b8ba67585aad68b9b9fda7279e69c307699`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d27bb3fd173781cf4aa8c000573dd19d67560e40b8d3fbeda1e8dccb421f579c`  
		Last Modified: Wed, 01 Jul 2020 00:19:52 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904999bb09b75919ca03f67a70d2a35158b27d69df0eccf5fea477d5bf4f6d5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d50033284bbf2d266f56a8f2b89a8b0a9cf5e9551b2cfb7e9310a7865c2c8ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:228fda428e977e94a9217a57b29b5b0bc3390f1672704f981ea97327281f0a5f`  
		Last Modified: Wed, 01 Jul 2020 00:19:51 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95dbe0b17ebfd63d3ff3126bdfb2b2563c09abac1e153667fd506fe16ff48cdc`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3caae4654ac48585a8fb3498155272a4fc11834530bd756163532c7869035a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0340322dd9ac8223b69a845ecf656fe382bb1764b559a6817748c6505040459a`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541de31fd9fbe59c99012142d3e1fbc01d00baeceb1cf4025c1bad60ce742d18`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 240.4 KB (240414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ae3d73e72ea4c0be00a0fc1a9239f8a48bbaa6838d98adfdbbfe38fda4e1ad`  
		Last Modified: Wed, 01 Jul 2020 00:19:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
