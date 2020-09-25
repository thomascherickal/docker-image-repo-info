<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.1.1`](#caddy211)
-	[`caddy:2.1.1-alpine`](#caddy211-alpine)
-	[`caddy:2.1.1-builder`](#caddy211-builder)
-	[`caddy:2.1.1-builder-alpine`](#caddy211-builder-alpine)
-	[`caddy:2.1.1-builder-windowsservercore-1809`](#caddy211-builder-windowsservercore-1809)
-	[`caddy:2.1.1-builder-windowsservercore-ltsc2016`](#caddy211-builder-windowsservercore-ltsc2016)
-	[`caddy:2.1.1-windowsservercore`](#caddy211-windowsservercore)
-	[`caddy:2.1.1-windowsservercore-1809`](#caddy211-windowsservercore-1809)
-	[`caddy:2.1.1-windowsservercore-ltsc2016`](#caddy211-windowsservercore-ltsc2016)
-	[`caddy:2.2.0`](#caddy220)
-	[`caddy:2.2.0-alpine`](#caddy220-alpine)
-	[`caddy:2.2.0-builder`](#caddy220-builder)
-	[`caddy:2.2.0-builder-alpine`](#caddy220-builder-alpine)
-	[`caddy:2.2.0-builder-windowsservercore-1809`](#caddy220-builder-windowsservercore-1809)
-	[`caddy:2.2.0-builder-windowsservercore-ltsc2016`](#caddy220-builder-windowsservercore-ltsc2016)
-	[`caddy:2.2.0-windowsservercore`](#caddy220-windowsservercore)
-	[`caddy:2.2.0-windowsservercore-1809`](#caddy220-windowsservercore-1809)
-	[`caddy:2.2.0-windowsservercore-ltsc2016`](#caddy220-windowsservercore-ltsc2016)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2016`](#caddy2-builder-windowsservercore-ltsc2016)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2016`](#caddy2-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:d9e3041657102dfd878f2c70893cb324cca11f9e1d22ad82692d2c4bb83f41c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

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

### `caddy:2` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:d9e3041657102dfd878f2c70893cb324cca11f9e1d22ad82692d2c4bb83f41c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

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

### `caddy:2.1.1` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
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
$ docker pull caddy@sha256:16450c5118cda1aa2b8934afd0c9fc93864413ae49c461127f512fe9826d68c4
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
$ docker pull caddy@sha256:c6a42d4224bcbc1aa0d2671eb97d2f06a439c36386eedc5d280f8d8cac870ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (306011968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eae05b9c152023f118a7b41498c3413fc036dd459dd8cb0b6d3f901e3ddad7b`
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
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:58 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:25:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:25:12 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:25:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:25:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:25:13 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:46:24 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:46:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:46:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:46:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:46:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:46:55 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:46:57 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:46:57 GMT
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
	-	`sha256:5d0547b08c8963faeee9d579d8351699f769179aa7a58ada0290e6ab8f5a676c`  
		Last Modified: Wed, 09 Sep 2020 22:30:12 GMT  
		Size: 107.4 MB (107371657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b6f0657434294654385190364b1a7c9af2a6f7b7ef0e821b8d51e20cdd8da5`  
		Last Modified: Wed, 09 Sep 2020 22:29:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f980c0941f345f6e2bea099934d861e844bc878396f9e95b425cdacf969a2815`  
		Last Modified: Wed, 09 Sep 2020 22:47:13 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e601915031b79952a33dafb7515134d728a30295c6f0c269bd6ed347753d6e`  
		Last Modified: Wed, 09 Sep 2020 22:47:14 GMT  
		Size: 8.3 MB (8310036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de90b62b6b63d79c1b0449a3b5b3ae59fe19f70cce318a51ddb32bcecb8305`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 3.0 MB (3018197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d779c3f8e871ce33b2daa7edc47e877d7eb18207a9707540088c581e49e764c`  
		Last Modified: Wed, 09 Sep 2020 22:47:46 GMT  
		Size: 184.2 MB (184230897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7817237c1f4eeca376d869f4f339d9631fea2a626190b431ddd23fa7135b54e`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff33af75dd2537d1113713133abb0aa2309dd380964987be7e08bda4f2d8475`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:90e5ec60900a30c987c06bd8351a60c3831e1f6174caa8acad53eaba9c1c058e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.8 MB (301787869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff83d67e33fd4e4345a625cbcaf782fb6631bb7e3acdde4c1b78e1ed7a39c39`
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
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:54:15 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:57:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:57:19 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:57:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:57:23 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:18:57 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:19:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:19:01 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:19:03 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:19:04 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:19:48 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:19:56 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:19:57 GMT
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
	-	`sha256:cd6fe6c5f0fa89cff72714190eb250d37035e32c7216624ea20cfcdfc88d8932`  
		Last Modified: Wed, 09 Sep 2020 23:02:32 GMT  
		Size: 103.7 MB (103712873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bd058112580f710efc27a0aae302bc22b6933011ca92545db5a513ddde4c0`  
		Last Modified: Wed, 09 Sep 2020 23:02:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd397f94f141bae6ded3b8214f6110d80dc00d0ecf9ddef507d79894a47919f`  
		Last Modified: Wed, 09 Sep 2020 23:20:14 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d09780d3f5ad562a835d8bb15c67e4bd59406c7425f41b7f98a790d082039f`  
		Last Modified: Wed, 09 Sep 2020 23:20:16 GMT  
		Size: 7.9 MB (7928854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60355ccb513fab7d8bb83c8cc017903818b391069f816e3a0279b299a3972f22`  
		Last Modified: Wed, 09 Sep 2020 23:20:13 GMT  
		Size: 3.0 MB (3022076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab0b979ca808d239596bf34c983260643fbd5374e4fa9ad61679fb632cbea1c`  
		Last Modified: Wed, 09 Sep 2020 23:20:57 GMT  
		Size: 184.2 MB (184236874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40612d06549d6b11fd1d0cf5cd146540e6ab04bb059e4c0a341163e29bbd386d`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ffbb030b4179d885102c4a784086e9546524fd618a5f8f098175cabdec5bbd`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7eefa86defbd314e38f66a52e2088430aa9849c52321c5de4031b8b525af3aab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb6f0c9bdc5fcee0387fbb1476e819c3b669cc1bd96063104004575f95bc2b`
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
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:05:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:07:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:07:51 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:07:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:07:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:07:54 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:30:49 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:30:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:30:52 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:30:55 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:30:56 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:31:44 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:31:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:31:52 GMT
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
	-	`sha256:189358c25ed3947ca4fd93936880bae2e9a32a62f75d865d03db0ce536130f63`  
		Last Modified: Wed, 09 Sep 2020 22:14:22 GMT  
		Size: 103.5 MB (103462777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a5f301bfa0a4263c5e4fd043d781161d2579b6d5ac42d3a18287f1452e4194`  
		Last Modified: Wed, 09 Sep 2020 22:13:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627fae0811bf183e71d577ae5c25b7231850907cf5657027a2276754993ad359`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f15eb32ecbdabe764b8485a4a137b40d9bb510b36fb58b19c4860b1aa3b66e`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 7.1 MB (7144998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9ac55041b3869f979a1080d8e43f8d238ba533c561e1003b54aacd2bce0b10`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 3.0 MB (3022109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990eaa3e8964d6482ef1e27a21997a4edc1a01d94e1a9b4c0a4dc1fbe3a9dc84`  
		Last Modified: Wed, 09 Sep 2020 22:33:01 GMT  
		Size: 184.2 MB (184240143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc787416c2c469678e1e5f622edf0b61d332cc35e224d63e818d50a488b6a2`  
		Last Modified: Wed, 09 Sep 2020 22:32:15 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b8026d3dfebac1b5186b3c3a99b251d0905e643e9d1f1606f4ee5e8dcad2f2`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:717015810b86bf461e53dc244b53947fbc7a1f71b64732f8a718a822e6b5187d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301563276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376db6534da4c0bfb8aad0f04b914f4758108b57b1ddec92d0f75b3fdf7b2c20`
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
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:22 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:10 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:14 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:07:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:07:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:07:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:07:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:07:30 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:15 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:22 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:23 GMT
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
	-	`sha256:1aee363a75d12710f67004978ba4509d1ddb769cc47ba518bc277ecd103a6b8d`  
		Last Modified: Wed, 09 Sep 2020 22:51:01 GMT  
		Size: 102.8 MB (102811724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab2d6f42095309ce47a6ec4edd38bd86aabe0fb28a18cb007652d42e0f19e0`  
		Last Modified: Wed, 09 Sep 2020 22:50:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5489d969be50d3033392e45f0052fb16b683933184e54bd6dc90a7836630f9bd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605dc1c7f70c44d1833597873e877f6c60ee04cba8abf125bf40e6c7d473dbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 8.5 MB (8499918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d068ddd7d6434e06055a366bc9e5252ebe01b49bf8b2d9877f9906db1294a`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 3.0 MB (3018223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcaf2776515e62eb5a9cf01d1c1631d613fb1080c601baa44c29770df447c04`  
		Last Modified: Wed, 09 Sep 2020 23:09:16 GMT  
		Size: 184.2 MB (184241320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430830f0fb8086c376793d765be00c6a226da704f9630a333e1a3018e9c5efbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a903bbf5561bf05e968292470a38298e42f48afbef9b0203954316e7fe6d8e8`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f4cb30c6502ec2ff6ec3fa211bb84c01b260969e892a3f8599edf31c5977cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (300951497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4440d71ff6b1d6f7f0ab958da228bc2d958e1ee40c863c011d7196d72c0a44`
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
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:26:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:29:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:29:52 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:29:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:30:39 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:01:13 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:01:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:01:31 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:01:45 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:01:53 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:24 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:34 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:43 GMT
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
	-	`sha256:ba569e5c85b1b70b3985f097dd79fee89c81c111899c623098e368323e560524`  
		Last Modified: Wed, 09 Sep 2020 22:44:05 GMT  
		Size: 101.7 MB (101676592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cb177af69484b6f3437a2174165ac7a6c677d76f72e742f049397fb1fe2df`  
		Last Modified: Wed, 09 Sep 2020 22:43:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18250f29498ec73e2ddfef536b10a494834e99da6b938037fecd9f94e386105`  
		Last Modified: Wed, 09 Sep 2020 23:09:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed76b1419d6b1a5c79669d485991765fb3e2e85ff1646a9a9881738e6f9e2d`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 8.9 MB (8920013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f641502fd10f29dac58992a2d912c15543f52beed8a2e94c366f048d75f82412`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 3.0 MB (3018870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428661f93ba3d47996eff0cfadaad0939e596d8c80418ed72c11118bef48b542`  
		Last Modified: Wed, 09 Sep 2020 23:09:39 GMT  
		Size: 184.2 MB (184244659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c8eddd4fb8576ce08a8d2c4d19ca69af18125ab0aea66e5ea209e9686f11ff`  
		Last Modified: Wed, 09 Sep 2020 23:09:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7c2fd8cee6e0b035ef2d5f127b71624a0047bd309476b3761549dbbc091bdc`  
		Last Modified: Wed, 09 Sep 2020 23:09:10 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c4c9e94d1f1fa36400a42c26efa6b0bb06b60072f31e2011c7ed1d6899e67fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305706045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d86f5ded96bbb8bedc72304d2f4ce10bb466e18c23f60926b7f81ad8bdd61ce`
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
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:55 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:07 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:08 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:04:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:04:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:04:25 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:04:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:04:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:04:43 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:04:51 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:04:51 GMT
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
	-	`sha256:c7e7f0b644229c4d22243efaf9cde7728d52c4624e9d48ab2d5174ec187de5f9`  
		Last Modified: Wed, 09 Sep 2020 22:48:16 GMT  
		Size: 107.3 MB (107254107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b1ab98332292b26f0fee8484fc91221c2e937011cbcd0fa39c2b7f8b32252e`  
		Last Modified: Wed, 09 Sep 2020 22:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532f23f71a0518243acc85fd6f986818a0731f1234eb2e447d27cbe9f0ad9cdf`  
		Last Modified: Wed, 09 Sep 2020 23:05:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbc25f41a54e52aa69fcedd6a1d68a07d7c2357cf2d3325a93729306cad2a44`  
		Last Modified: Wed, 09 Sep 2020 23:05:07 GMT  
		Size: 8.4 MB (8352244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc2c684cdfce8879b83944ce50659293c1672ef6f2289aeae6d5e26105ed53`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 3.0 MB (3018172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ccaf1327d9e8c98f2135737060be2354164f2df682f4859dded7b22eb77fa6`  
		Last Modified: Wed, 09 Sep 2020 23:05:22 GMT  
		Size: 184.2 MB (184231058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89169387514d2f97acab2cb25524f5527d305110cd42e754b3c8a8c476b99962`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ad4ec30dc130d7bf579221c2331ee49316addfd281e3d3dc1c38c9a1b5bee`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-builder-alpine`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.1.1-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.1.1-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:40c4f77513048ee7e05ee01fb89d360e22b13325c3daaffca57dee62c72b575d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:54fc1c11a9a4de45c0e3b30aa2702ac0e55d355cd47e3f7f4fbfdc475bc6c132
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:deb60a2701067b98424a7cc203f79a61a9f41d6b772df3b6c0ba34236cce1c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.2.0`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-alpine`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-builder`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-builder-alpine`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-windowsservercore`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2.2.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

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
$ docker pull caddy@sha256:16450c5118cda1aa2b8934afd0c9fc93864413ae49c461127f512fe9826d68c4
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
$ docker pull caddy@sha256:c6a42d4224bcbc1aa0d2671eb97d2f06a439c36386eedc5d280f8d8cac870ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (306011968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eae05b9c152023f118a7b41498c3413fc036dd459dd8cb0b6d3f901e3ddad7b`
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
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:58 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:25:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:25:12 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:25:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:25:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:25:13 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:46:24 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:46:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:46:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:46:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:46:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:46:55 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:46:57 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:46:57 GMT
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
	-	`sha256:5d0547b08c8963faeee9d579d8351699f769179aa7a58ada0290e6ab8f5a676c`  
		Last Modified: Wed, 09 Sep 2020 22:30:12 GMT  
		Size: 107.4 MB (107371657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b6f0657434294654385190364b1a7c9af2a6f7b7ef0e821b8d51e20cdd8da5`  
		Last Modified: Wed, 09 Sep 2020 22:29:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f980c0941f345f6e2bea099934d861e844bc878396f9e95b425cdacf969a2815`  
		Last Modified: Wed, 09 Sep 2020 22:47:13 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e601915031b79952a33dafb7515134d728a30295c6f0c269bd6ed347753d6e`  
		Last Modified: Wed, 09 Sep 2020 22:47:14 GMT  
		Size: 8.3 MB (8310036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de90b62b6b63d79c1b0449a3b5b3ae59fe19f70cce318a51ddb32bcecb8305`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 3.0 MB (3018197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d779c3f8e871ce33b2daa7edc47e877d7eb18207a9707540088c581e49e764c`  
		Last Modified: Wed, 09 Sep 2020 22:47:46 GMT  
		Size: 184.2 MB (184230897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7817237c1f4eeca376d869f4f339d9631fea2a626190b431ddd23fa7135b54e`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff33af75dd2537d1113713133abb0aa2309dd380964987be7e08bda4f2d8475`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:90e5ec60900a30c987c06bd8351a60c3831e1f6174caa8acad53eaba9c1c058e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.8 MB (301787869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff83d67e33fd4e4345a625cbcaf782fb6631bb7e3acdde4c1b78e1ed7a39c39`
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
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:54:15 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:57:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:57:19 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:57:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:57:23 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:18:57 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:19:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:19:01 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:19:03 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:19:04 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:19:48 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:19:56 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:19:57 GMT
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
	-	`sha256:cd6fe6c5f0fa89cff72714190eb250d37035e32c7216624ea20cfcdfc88d8932`  
		Last Modified: Wed, 09 Sep 2020 23:02:32 GMT  
		Size: 103.7 MB (103712873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bd058112580f710efc27a0aae302bc22b6933011ca92545db5a513ddde4c0`  
		Last Modified: Wed, 09 Sep 2020 23:02:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd397f94f141bae6ded3b8214f6110d80dc00d0ecf9ddef507d79894a47919f`  
		Last Modified: Wed, 09 Sep 2020 23:20:14 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d09780d3f5ad562a835d8bb15c67e4bd59406c7425f41b7f98a790d082039f`  
		Last Modified: Wed, 09 Sep 2020 23:20:16 GMT  
		Size: 7.9 MB (7928854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60355ccb513fab7d8bb83c8cc017903818b391069f816e3a0279b299a3972f22`  
		Last Modified: Wed, 09 Sep 2020 23:20:13 GMT  
		Size: 3.0 MB (3022076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab0b979ca808d239596bf34c983260643fbd5374e4fa9ad61679fb632cbea1c`  
		Last Modified: Wed, 09 Sep 2020 23:20:57 GMT  
		Size: 184.2 MB (184236874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40612d06549d6b11fd1d0cf5cd146540e6ab04bb059e4c0a341163e29bbd386d`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ffbb030b4179d885102c4a784086e9546524fd618a5f8f098175cabdec5bbd`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7eefa86defbd314e38f66a52e2088430aa9849c52321c5de4031b8b525af3aab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb6f0c9bdc5fcee0387fbb1476e819c3b669cc1bd96063104004575f95bc2b`
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
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:05:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:07:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:07:51 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:07:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:07:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:07:54 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:30:49 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:30:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:30:52 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:30:55 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:30:56 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:31:44 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:31:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:31:52 GMT
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
	-	`sha256:189358c25ed3947ca4fd93936880bae2e9a32a62f75d865d03db0ce536130f63`  
		Last Modified: Wed, 09 Sep 2020 22:14:22 GMT  
		Size: 103.5 MB (103462777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a5f301bfa0a4263c5e4fd043d781161d2579b6d5ac42d3a18287f1452e4194`  
		Last Modified: Wed, 09 Sep 2020 22:13:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627fae0811bf183e71d577ae5c25b7231850907cf5657027a2276754993ad359`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f15eb32ecbdabe764b8485a4a137b40d9bb510b36fb58b19c4860b1aa3b66e`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 7.1 MB (7144998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9ac55041b3869f979a1080d8e43f8d238ba533c561e1003b54aacd2bce0b10`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 3.0 MB (3022109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990eaa3e8964d6482ef1e27a21997a4edc1a01d94e1a9b4c0a4dc1fbe3a9dc84`  
		Last Modified: Wed, 09 Sep 2020 22:33:01 GMT  
		Size: 184.2 MB (184240143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc787416c2c469678e1e5f622edf0b61d332cc35e224d63e818d50a488b6a2`  
		Last Modified: Wed, 09 Sep 2020 22:32:15 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b8026d3dfebac1b5186b3c3a99b251d0905e643e9d1f1606f4ee5e8dcad2f2`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:717015810b86bf461e53dc244b53947fbc7a1f71b64732f8a718a822e6b5187d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301563276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376db6534da4c0bfb8aad0f04b914f4758108b57b1ddec92d0f75b3fdf7b2c20`
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
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:22 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:10 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:14 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:07:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:07:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:07:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:07:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:07:30 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:15 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:22 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:23 GMT
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
	-	`sha256:1aee363a75d12710f67004978ba4509d1ddb769cc47ba518bc277ecd103a6b8d`  
		Last Modified: Wed, 09 Sep 2020 22:51:01 GMT  
		Size: 102.8 MB (102811724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab2d6f42095309ce47a6ec4edd38bd86aabe0fb28a18cb007652d42e0f19e0`  
		Last Modified: Wed, 09 Sep 2020 22:50:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5489d969be50d3033392e45f0052fb16b683933184e54bd6dc90a7836630f9bd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605dc1c7f70c44d1833597873e877f6c60ee04cba8abf125bf40e6c7d473dbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 8.5 MB (8499918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d068ddd7d6434e06055a366bc9e5252ebe01b49bf8b2d9877f9906db1294a`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 3.0 MB (3018223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcaf2776515e62eb5a9cf01d1c1631d613fb1080c601baa44c29770df447c04`  
		Last Modified: Wed, 09 Sep 2020 23:09:16 GMT  
		Size: 184.2 MB (184241320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430830f0fb8086c376793d765be00c6a226da704f9630a333e1a3018e9c5efbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a903bbf5561bf05e968292470a38298e42f48afbef9b0203954316e7fe6d8e8`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f4cb30c6502ec2ff6ec3fa211bb84c01b260969e892a3f8599edf31c5977cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (300951497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4440d71ff6b1d6f7f0ab958da228bc2d958e1ee40c863c011d7196d72c0a44`
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
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:26:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:29:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:29:52 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:29:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:30:39 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:01:13 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:01:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:01:31 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:01:45 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:01:53 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:24 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:34 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:43 GMT
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
	-	`sha256:ba569e5c85b1b70b3985f097dd79fee89c81c111899c623098e368323e560524`  
		Last Modified: Wed, 09 Sep 2020 22:44:05 GMT  
		Size: 101.7 MB (101676592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cb177af69484b6f3437a2174165ac7a6c677d76f72e742f049397fb1fe2df`  
		Last Modified: Wed, 09 Sep 2020 22:43:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18250f29498ec73e2ddfef536b10a494834e99da6b938037fecd9f94e386105`  
		Last Modified: Wed, 09 Sep 2020 23:09:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed76b1419d6b1a5c79669d485991765fb3e2e85ff1646a9a9881738e6f9e2d`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 8.9 MB (8920013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f641502fd10f29dac58992a2d912c15543f52beed8a2e94c366f048d75f82412`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 3.0 MB (3018870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428661f93ba3d47996eff0cfadaad0939e596d8c80418ed72c11118bef48b542`  
		Last Modified: Wed, 09 Sep 2020 23:09:39 GMT  
		Size: 184.2 MB (184244659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c8eddd4fb8576ce08a8d2c4d19ca69af18125ab0aea66e5ea209e9686f11ff`  
		Last Modified: Wed, 09 Sep 2020 23:09:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7c2fd8cee6e0b035ef2d5f127b71624a0047bd309476b3761549dbbc091bdc`  
		Last Modified: Wed, 09 Sep 2020 23:09:10 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c4c9e94d1f1fa36400a42c26efa6b0bb06b60072f31e2011c7ed1d6899e67fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305706045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d86f5ded96bbb8bedc72304d2f4ce10bb466e18c23f60926b7f81ad8bdd61ce`
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
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:55 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:07 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:08 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:04:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:04:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:04:25 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:04:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:04:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:04:43 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:04:51 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:04:51 GMT
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
	-	`sha256:c7e7f0b644229c4d22243efaf9cde7728d52c4624e9d48ab2d5174ec187de5f9`  
		Last Modified: Wed, 09 Sep 2020 22:48:16 GMT  
		Size: 107.3 MB (107254107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b1ab98332292b26f0fee8484fc91221c2e937011cbcd0fa39c2b7f8b32252e`  
		Last Modified: Wed, 09 Sep 2020 22:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532f23f71a0518243acc85fd6f986818a0731f1234eb2e447d27cbe9f0ad9cdf`  
		Last Modified: Wed, 09 Sep 2020 23:05:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbc25f41a54e52aa69fcedd6a1d68a07d7c2357cf2d3325a93729306cad2a44`  
		Last Modified: Wed, 09 Sep 2020 23:05:07 GMT  
		Size: 8.4 MB (8352244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc2c684cdfce8879b83944ce50659293c1672ef6f2289aeae6d5e26105ed53`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 3.0 MB (3018172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ccaf1327d9e8c98f2135737060be2354164f2df682f4859dded7b22eb77fa6`  
		Last Modified: Wed, 09 Sep 2020 23:05:22 GMT  
		Size: 184.2 MB (184231058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89169387514d2f97acab2cb25524f5527d305110cd42e754b3c8a8c476b99962`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ad4ec30dc130d7bf579221c2331ee49316addfd281e3d3dc1c38c9a1b5bee`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:40c4f77513048ee7e05ee01fb89d360e22b13325c3daaffca57dee62c72b575d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:54fc1c11a9a4de45c0e3b30aa2702ac0e55d355cd47e3f7f4fbfdc475bc6c132
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:deb60a2701067b98424a7cc203f79a61a9f41d6b772df3b6c0ba34236cce1c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
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
$ docker pull caddy@sha256:16450c5118cda1aa2b8934afd0c9fc93864413ae49c461127f512fe9826d68c4
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
$ docker pull caddy@sha256:c6a42d4224bcbc1aa0d2671eb97d2f06a439c36386eedc5d280f8d8cac870ac2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (306011968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eae05b9c152023f118a7b41498c3413fc036dd459dd8cb0b6d3f901e3ddad7b`
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
# Tue, 01 Sep 2020 00:40:24 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:22:58 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:25:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:25:12 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:25:13 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:25:13 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:25:13 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:46:24 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:46:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:46:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:46:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:46:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:46:55 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:46:57 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:46:57 GMT
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
	-	`sha256:5d0547b08c8963faeee9d579d8351699f769179aa7a58ada0290e6ab8f5a676c`  
		Last Modified: Wed, 09 Sep 2020 22:30:12 GMT  
		Size: 107.4 MB (107371657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b6f0657434294654385190364b1a7c9af2a6f7b7ef0e821b8d51e20cdd8da5`  
		Last Modified: Wed, 09 Sep 2020 22:29:55 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f980c0941f345f6e2bea099934d861e844bc878396f9e95b425cdacf969a2815`  
		Last Modified: Wed, 09 Sep 2020 22:47:13 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e601915031b79952a33dafb7515134d728a30295c6f0c269bd6ed347753d6e`  
		Last Modified: Wed, 09 Sep 2020 22:47:14 GMT  
		Size: 8.3 MB (8310036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55de90b62b6b63d79c1b0449a3b5b3ae59fe19f70cce318a51ddb32bcecb8305`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 3.0 MB (3018197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d779c3f8e871ce33b2daa7edc47e877d7eb18207a9707540088c581e49e764c`  
		Last Modified: Wed, 09 Sep 2020 22:47:46 GMT  
		Size: 184.2 MB (184230897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7817237c1f4eeca376d869f4f339d9631fea2a626190b431ddd23fa7135b54e`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff33af75dd2537d1113713133abb0aa2309dd380964987be7e08bda4f2d8475`  
		Last Modified: Wed, 09 Sep 2020 22:47:12 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:90e5ec60900a30c987c06bd8351a60c3831e1f6174caa8acad53eaba9c1c058e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.8 MB (301787869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff83d67e33fd4e4345a625cbcaf782fb6631bb7e3acdde4c1b78e1ed7a39c39`
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
# Mon, 31 Aug 2020 23:51:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:54:15 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:57:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:57:19 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:57:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:57:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:57:23 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:18:57 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:19:00 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:19:01 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:19:03 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:19:04 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:19:48 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:19:56 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:19:57 GMT
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
	-	`sha256:cd6fe6c5f0fa89cff72714190eb250d37035e32c7216624ea20cfcdfc88d8932`  
		Last Modified: Wed, 09 Sep 2020 23:02:32 GMT  
		Size: 103.7 MB (103712873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186bd058112580f710efc27a0aae302bc22b6933011ca92545db5a513ddde4c0`  
		Last Modified: Wed, 09 Sep 2020 23:02:01 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd397f94f141bae6ded3b8214f6110d80dc00d0ecf9ddef507d79894a47919f`  
		Last Modified: Wed, 09 Sep 2020 23:20:14 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d09780d3f5ad562a835d8bb15c67e4bd59406c7425f41b7f98a790d082039f`  
		Last Modified: Wed, 09 Sep 2020 23:20:16 GMT  
		Size: 7.9 MB (7928854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60355ccb513fab7d8bb83c8cc017903818b391069f816e3a0279b299a3972f22`  
		Last Modified: Wed, 09 Sep 2020 23:20:13 GMT  
		Size: 3.0 MB (3022076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab0b979ca808d239596bf34c983260643fbd5374e4fa9ad61679fb632cbea1c`  
		Last Modified: Wed, 09 Sep 2020 23:20:57 GMT  
		Size: 184.2 MB (184236874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40612d06549d6b11fd1d0cf5cd146540e6ab04bb059e4c0a341163e29bbd386d`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ffbb030b4179d885102c4a784086e9546524fd618a5f8f098175cabdec5bbd`  
		Last Modified: Wed, 09 Sep 2020 23:20:12 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:7eefa86defbd314e38f66a52e2088430aa9849c52321c5de4031b8b525af3aab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **300.6 MB (300559812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9acb6f0c9bdc5fcee0387fbb1476e819c3b669cc1bd96063104004575f95bc2b`
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
# Tue, 01 Sep 2020 00:46:57 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:05:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:07:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:07:51 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:07:52 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:07:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:07:54 GMT
WORKDIR /go
# Wed, 09 Sep 2020 22:30:49 GMT
WORKDIR /src
# Wed, 09 Sep 2020 22:30:52 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 22:30:52 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 22:30:55 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 22:30:56 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 22:31:44 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 22:31:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 22:31:52 GMT
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
	-	`sha256:189358c25ed3947ca4fd93936880bae2e9a32a62f75d865d03db0ce536130f63`  
		Last Modified: Wed, 09 Sep 2020 22:14:22 GMT  
		Size: 103.5 MB (103462777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a5f301bfa0a4263c5e4fd043d781161d2579b6d5ac42d3a18287f1452e4194`  
		Last Modified: Wed, 09 Sep 2020 22:13:50 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:627fae0811bf183e71d577ae5c25b7231850907cf5657027a2276754993ad359`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f15eb32ecbdabe764b8485a4a137b40d9bb510b36fb58b19c4860b1aa3b66e`  
		Last Modified: Wed, 09 Sep 2020 22:32:17 GMT  
		Size: 7.1 MB (7144998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9ac55041b3869f979a1080d8e43f8d238ba533c561e1003b54aacd2bce0b10`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 3.0 MB (3022109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990eaa3e8964d6482ef1e27a21997a4edc1a01d94e1a9b4c0a4dc1fbe3a9dc84`  
		Last Modified: Wed, 09 Sep 2020 22:33:01 GMT  
		Size: 184.2 MB (184240143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc787416c2c469678e1e5f622edf0b61d332cc35e224d63e818d50a488b6a2`  
		Last Modified: Wed, 09 Sep 2020 22:32:15 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b8026d3dfebac1b5186b3c3a99b251d0905e643e9d1f1606f4ee5e8dcad2f2`  
		Last Modified: Wed, 09 Sep 2020 22:32:16 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:717015810b86bf461e53dc244b53947fbc7a1f71b64732f8a718a822e6b5187d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301563276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:376db6534da4c0bfb8aad0f04b914f4758108b57b1ddec92d0f75b3fdf7b2c20`
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
# Mon, 31 Aug 2020 23:59:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:22 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:10 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:14 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:14 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:07:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:07:25 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:07:26 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:07:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:07:30 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:15 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:22 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:23 GMT
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
	-	`sha256:1aee363a75d12710f67004978ba4509d1ddb769cc47ba518bc277ecd103a6b8d`  
		Last Modified: Wed, 09 Sep 2020 22:51:01 GMT  
		Size: 102.8 MB (102811724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffab2d6f42095309ce47a6ec4edd38bd86aabe0fb28a18cb007652d42e0f19e0`  
		Last Modified: Wed, 09 Sep 2020 22:50:31 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5489d969be50d3033392e45f0052fb16b683933184e54bd6dc90a7836630f9bd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605dc1c7f70c44d1833597873e877f6c60ee04cba8abf125bf40e6c7d473dbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:40 GMT  
		Size: 8.5 MB (8499918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26d068ddd7d6434e06055a366bc9e5252ebe01b49bf8b2d9877f9906db1294a`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 3.0 MB (3018223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcaf2776515e62eb5a9cf01d1c1631d613fb1080c601baa44c29770df447c04`  
		Last Modified: Wed, 09 Sep 2020 23:09:16 GMT  
		Size: 184.2 MB (184241320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430830f0fb8086c376793d765be00c6a226da704f9630a333e1a3018e9c5efbd`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a903bbf5561bf05e968292470a38298e42f48afbef9b0203954316e7fe6d8e8`  
		Last Modified: Wed, 09 Sep 2020 23:08:39 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:3f4cb30c6502ec2ff6ec3fa211bb84c01b260969e892a3f8599edf31c5977cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (300951497 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4440d71ff6b1d6f7f0ab958da228bc2d958e1ee40c863c011d7196d72c0a44`
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
# Tue, 01 Sep 2020 01:38:15 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:26:40 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:29:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:29:52 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:29:59 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:30:39 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:01:13 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:01:26 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:01:31 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:01:45 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:01:53 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:08:24 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:08:34 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:08:43 GMT
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
	-	`sha256:ba569e5c85b1b70b3985f097dd79fee89c81c111899c623098e368323e560524`  
		Last Modified: Wed, 09 Sep 2020 22:44:05 GMT  
		Size: 101.7 MB (101676592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826cb177af69484b6f3437a2174165ac7a6c677d76f72e742f049397fb1fe2df`  
		Last Modified: Wed, 09 Sep 2020 22:43:44 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18250f29498ec73e2ddfef536b10a494834e99da6b938037fecd9f94e386105`  
		Last Modified: Wed, 09 Sep 2020 23:09:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ed76b1419d6b1a5c79669d485991765fb3e2e85ff1646a9a9881738e6f9e2d`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 8.9 MB (8920013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f641502fd10f29dac58992a2d912c15543f52beed8a2e94c366f048d75f82412`  
		Last Modified: Wed, 09 Sep 2020 23:09:13 GMT  
		Size: 3.0 MB (3018870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:428661f93ba3d47996eff0cfadaad0939e596d8c80418ed72c11118bef48b542`  
		Last Modified: Wed, 09 Sep 2020 23:09:39 GMT  
		Size: 184.2 MB (184244659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c8eddd4fb8576ce08a8d2c4d19ca69af18125ab0aea66e5ea209e9686f11ff`  
		Last Modified: Wed, 09 Sep 2020 23:09:12 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7c2fd8cee6e0b035ef2d5f127b71624a0047bd309476b3761549dbbc091bdc`  
		Last Modified: Wed, 09 Sep 2020 23:09:10 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:1c4c9e94d1f1fa36400a42c26efa6b0bb06b60072f31e2011c7ed1d6899e67fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.7 MB (305706045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d86f5ded96bbb8bedc72304d2f4ce10bb466e18c23f60926b7f81ad8bdd61ce`
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
# Mon, 31 Aug 2020 23:53:42 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:43:55 GMT
ENV GOLANG_VERSION=1.14.9
# Wed, 09 Sep 2020 22:45:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.9.src.tar.gz'; 	sha256='c687c848cc09bcabf2b5e534c3fc4259abebbfc9014dd05a1a2dc6106f404554'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Wed, 09 Sep 2020 22:45:07 GMT
ENV GOPATH=/go
# Wed, 09 Sep 2020 22:45:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Sep 2020 22:45:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 09 Sep 2020 22:45:08 GMT
WORKDIR /go
# Wed, 09 Sep 2020 23:04:23 GMT
WORKDIR /src
# Wed, 09 Sep 2020 23:04:24 GMT
RUN apk add --no-cache     git     ca-certificates
# Wed, 09 Sep 2020 23:04:25 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Wed, 09 Sep 2020 23:04:28 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Wed, 09 Sep 2020 23:04:28 GMT
WORKDIR /src/caddy/cmd/caddy
# Wed, 09 Sep 2020 23:04:43 GMT
RUN go get -d ./...
# Wed, 09 Sep 2020 23:04:51 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Wed, 09 Sep 2020 23:04:51 GMT
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
	-	`sha256:c7e7f0b644229c4d22243efaf9cde7728d52c4624e9d48ab2d5174ec187de5f9`  
		Last Modified: Wed, 09 Sep 2020 22:48:16 GMT  
		Size: 107.3 MB (107254107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b1ab98332292b26f0fee8484fc91221c2e937011cbcd0fa39c2b7f8b32252e`  
		Last Modified: Wed, 09 Sep 2020 22:48:03 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:532f23f71a0518243acc85fd6f986818a0731f1234eb2e447d27cbe9f0ad9cdf`  
		Last Modified: Wed, 09 Sep 2020 23:05:08 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fbc25f41a54e52aa69fcedd6a1d68a07d7c2357cf2d3325a93729306cad2a44`  
		Last Modified: Wed, 09 Sep 2020 23:05:07 GMT  
		Size: 8.4 MB (8352244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0dc2c684cdfce8879b83944ce50659293c1672ef6f2289aeae6d5e26105ed53`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 3.0 MB (3018172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ccaf1327d9e8c98f2135737060be2354164f2df682f4859dded7b22eb77fa6`  
		Last Modified: Wed, 09 Sep 2020 23:05:22 GMT  
		Size: 184.2 MB (184231058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89169387514d2f97acab2cb25524f5527d305110cd42e754b3c8a8c476b99962`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ad4ec30dc130d7bf579221c2331ee49316addfd281e3d3dc1c38c9a1b5bee`  
		Last Modified: Wed, 09 Sep 2020 23:05:06 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `caddy:latest`

```console
$ docker pull caddy@sha256:d9e3041657102dfd878f2c70893cb324cca11f9e1d22ad82692d2c4bb83f41c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

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

### `caddy:latest` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:40c4f77513048ee7e05ee01fb89d360e22b13325c3daaffca57dee62c72b575d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:54fc1c11a9a4de45c0e3b30aa2702ac0e55d355cd47e3f7f4fbfdc475bc6c132
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull caddy@sha256:6fdda8066ebb2cfcbb65432af3efad7ecef7f89d4b5a2e0b325692d95ea4e3b9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2378390339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29a3b078a6f6a6627a26f04efe9831b83aa9ce0bbb6249c8b0f92d7a50881c02`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 19:53:27 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 19:54:04 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 19:54:05 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 19:54:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 19:54:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 19:54:37 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 19:54:38 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 19:54:39 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 19:54:40 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 19:54:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 19:54:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 19:54:43 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 19:54:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 19:54:45 GMT
EXPOSE 80
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 443
# Wed, 09 Sep 2020 19:54:46 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:25:17 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:25:18 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c325b871c49357c593876a98f079c074af004dee2cb9cf372880b2cd25fd6a0c`  
		Last Modified: Wed, 09 Sep 2020 20:29:31 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc5eb7f2e0263c6213fc9423cf6eb719de3f7c849643ccdabec913b618f41ad`  
		Last Modified: Wed, 09 Sep 2020 20:29:39 GMT  
		Size: 9.1 MB (9137985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5a77a42e4acde519b57884bb795f3dc263fa0169242832aa756ec95c04dddd`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ef31d9b01fa7c0d2d8b5dc3eb4d389001034b74d7d472cc951df62d115118`  
		Last Modified: Wed, 09 Sep 2020 20:29:48 GMT  
		Size: 17.7 MB (17672633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665a7d301d80ee07b021c74d836eb43352e05ce53a3480b8d9e24d99186bbfbf`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0770a21ef08a40302425e6476fe8c78962bc91e1f2e01ce71d58b44d1eec27ff`  
		Last Modified: Wed, 09 Sep 2020 20:29:29 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74371eb56f1a9b6b6e10b2915999a33587eecd4cf57dc6442471c378718c1062`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3517d1abc56a70595cf5ae149a9f2843e8fa9eaa2c2f3c9e793cacc8e117dc3`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4bf115547c84fde7026e799220c3a33867058af6f6b469f7f6cad4fb501342`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ba56b6ad310ca4acd04b36bab15c11509edd717eacc8a7a31c575becf2e58c`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8e5887ab35d7d9526248c8ba42cd34560054c2eda04112f03bbb2c7051df82`  
		Last Modified: Wed, 09 Sep 2020 20:29:26 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ced70216aec7f6562500c53e1cb318c4f5fbd754b45dfd4778796eddcc3f44bf`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064b47540d3a0413e187206009b7420d041bc2abe86a2bdb159421da8a76e63`  
		Last Modified: Wed, 09 Sep 2020 20:29:24 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370539f66a716c49521cd612333716543831af692859d7406721cef7ac87476d`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c29ac445b054afa01e8bd41bdb11ba36d5af91e515aaf7abe5a6a156d838b4`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173743838549e9d6d35bf843fd1d0d578b7ff6f4353e4e14c9b62ac16d750efb`  
		Last Modified: Wed, 09 Sep 2020 20:29:23 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2116539be5612b7b677cc16f59fd8f7268ad3b1bea415498c4b31c99e1ca4565`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaed27ebe4f3042ae55963898c25ebf1f39d9e362ba02b80ddcefd0f40f3146`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cc079d30d61f51e726e25d5f65fad824d0749aefa98e25d25b1562b8785c753`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f7fdcbced701ca09049814e389bdab25b50586d869b3191093f5e9066efcd0`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 285.9 KB (285915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2630294809bc2c1fcd1b1976547723b64c5e7ed91f008f6f7ef23c871474a7fa`  
		Last Modified: Wed, 09 Sep 2020 20:29:21 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:deb60a2701067b98424a7cc203f79a61a9f41d6b772df3b6c0ba34236cce1c06
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3930; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3930; amd64

```console
$ docker pull caddy@sha256:c399072135a67ae1bf41ddf60b732de7e9d1513000021162c25f1a1471c07f95
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5772293185 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb680f013a85014fccf399ba08c16d449ca381f1a5154276bc2b49470ac8f942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 08 Sep 2020 19:31:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 20:25:23 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 09 Sep 2020 20:26:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Sep 2020 20:26:38 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 09 Sep 2020 20:28:00 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Sep 2020 20:28:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Sep 2020 20:28:02 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Sep 2020 20:28:03 GMT
VOLUME [c:/config]
# Wed, 09 Sep 2020 20:28:04 GMT
VOLUME [c:/data]
# Wed, 09 Sep 2020 20:28:05 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 09 Sep 2020 20:28:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Sep 2020 20:28:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Sep 2020 20:28:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Sep 2020 20:28:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Sep 2020 20:28:10 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Sep 2020 20:28:11 GMT
EXPOSE 80
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 443
# Wed, 09 Sep 2020 20:28:12 GMT
EXPOSE 2019
# Wed, 09 Sep 2020 20:28:52 GMT
RUN caddy version
# Wed, 09 Sep 2020 20:28:53 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8f6f82df7cca9113965bd35d2921a651250266aa7a3a9df6a0a42e8c005f1333`  
		Last Modified: Tue, 08 Sep 2020 19:53:55 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a449faf0a811f283e675b95675b755ed5caeaf09c377b034b4730f6451aa51`  
		Last Modified: Wed, 09 Sep 2020 20:30:15 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3226e2cab68073e9c97dacb0b90ecf5fec0142f1690d3ce6268fbe7236afc5`  
		Last Modified: Wed, 09 Sep 2020 20:30:24 GMT  
		Size: 9.9 MB (9897398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761d232ac4fd149d90e5347a5bd38a319bfb55a301c1a111b6503356911322b8`  
		Last Modified: Wed, 09 Sep 2020 20:30:13 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c767daadf962c116a6b9c0a3515446a8b285066125527c4222daf121a40a2ad7`  
		Last Modified: Wed, 09 Sep 2020 20:30:18 GMT  
		Size: 22.9 MB (22872196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b987d95380ab88f45603aaaed62a622130e9e3fdfaf920f4f75bce40bae1a635`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802d13151eefdd188af28474ad33dc2a1c63c9403c1ed769da6d40b0e54a806`  
		Last Modified: Wed, 09 Sep 2020 20:30:12 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26007a9ef743163079afd033ec88dc054a50a1691ceb86abf06c3027fb4e5960`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df9545735b7e2fd0e54384a7d867cb94d15f421965a72064960cd7b8884700`  
		Last Modified: Wed, 09 Sep 2020 20:30:10 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91bd9d5351e7b6f497b9506e976a1e9a722f4c1e3a99e8a476e1a7bda5fd3f4`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8fdc70bbab6bb9610494fc861f433042c460157a65717802379ddf4da12e81e`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663a9f158ac2229e071d383cec9f621fd28f6b0652215f5b4b4450b58dc68a1`  
		Last Modified: Wed, 09 Sep 2020 20:30:09 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1a243df49719e70d6a15b261449414bc069ffdd04a552563e129e402e3cc129`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff2d8f5da7ba33566df13bc15bfa47c970f50f27d4a373e0ad2085ff6435ffb4`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05d556209c77456fc89bd1484059081409259c5946aa6fc367179ceaca4674d`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1f5c7e3672363102592a251895dd3aebe3b1ffb623b0b03712525571abf474`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1deca8290b7668c1e16e216ed2040490186e8013ee60f992ab46347e92ccfde5`  
		Last Modified: Wed, 09 Sep 2020 20:30:07 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713887e22bbfa9481da702fba31404d11d79a9952c0ba63e8db952c7ab063b6d`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087dd32d3c1a6a7665699ccc8a08848a94b90c86b352804c29de30be754c7508`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0202c220609d5cf8ed133c56b31a32168cf749346cdd1453edc215f62cd09a8f`  
		Last Modified: Wed, 09 Sep 2020 20:30:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0823fb990936970db69fcf021f5cf762bcf64bf24669f09449c6f578ddd6f2`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 247.5 KB (247496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab51024f33e212313a4c9be7fb692bf2a599f8b8095c80c62127268d4ce704d3`  
		Last Modified: Wed, 09 Sep 2020 20:30:04 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
