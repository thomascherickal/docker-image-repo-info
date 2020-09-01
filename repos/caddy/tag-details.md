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
$ docker pull caddy@sha256:76e5b24fe40ee203c6da262f5d5a2661fcc4b7c49ad0e2c13d10bd40a70af476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

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

### `caddy:2` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1`

```console
$ docker pull caddy@sha256:76e5b24fe40ee203c6da262f5d5a2661fcc4b7c49ad0e2c13d10bd40a70af476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

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

### `caddy:2.1.1` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull caddy@sha256:414a95b02fe627ddb1c5644f51b1cdcfc75cfdded416424005e307e834d5f086
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
$ docker pull caddy@sha256:0fc57db9e46d2a71ee3903d22b5ce41e96cdc7a4f17f1c60f654a752b7299a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331162586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48efad8af5ceb779c7ff2fe387448d1d710ffc33d9b3f9abc95d885cd1f64b47`
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
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
# Fri, 07 Aug 2020 03:13:30 GMT
WORKDIR /src
# Fri, 07 Aug 2020 03:13:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 03:13:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 03:13:33 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 03:13:34 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 03:13:49 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 03:13:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 03:13:50 GMT
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
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fe5626f0254b9f60f5f61a291f5046b02ccfbc3f7081b0a44dddbca1397d`  
		Last Modified: Fri, 07 Aug 2020 03:14:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f972bf098f3488dd8a94d2eae2bcb6fc7a10b36175bcccca81baeb51fba4e9`  
		Last Modified: Fri, 07 Aug 2020 03:14:03 GMT  
		Size: 8.3 MB (8310028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bcf269b3e113e083f6a305bff186764723167a9b9625f602894d9cdd105c9a`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 3.0 MB (3022872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe8c223c437ec7b5d6ac8dfce77a26db0a34330288c7d0dbe3081116fe63db`  
		Last Modified: Fri, 07 Aug 2020 03:14:28 GMT  
		Size: 184.2 MB (184231010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35266c5be392980f82d35b0575940e3625d38bd55e3c03ca95e9dbd254b875eb`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb543dcf1b950699168feb583f397202802260bd84ef2c230f752539701b30fd`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:982248ee8c889b1765b1481b67ed5d16180a4ff6e82616d8dc82d56484a99742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.7 MB (301748871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eaed8f6193bdd4f5d28ddfbac079c84ae0260c92d2d9dd4016e87240089423d`
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
# Mon, 31 Aug 2020 23:55:22 GMT
ENV GOLANG_VERSION=1.14.7
# Tue, 01 Sep 2020 00:03:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 01 Sep 2020 00:03:34 GMT
ENV GOPATH=/go
# Tue, 01 Sep 2020 00:03:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Sep 2020 00:03:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Sep 2020 00:03:40 GMT
WORKDIR /go
# Tue, 01 Sep 2020 05:03:15 GMT
WORKDIR /src
# Tue, 01 Sep 2020 05:03:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 05:03:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 05:04:40 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 05:04:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 05:06:45 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 05:07:00 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 05:07:07 GMT
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
	-	`sha256:d80d870b4111d9793e4a962df54668501236ab71f0b3bd501fe19d8832d95bd2`  
		Last Modified: Tue, 01 Sep 2020 00:33:29 GMT  
		Size: 103.7 MB (103670838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbe42781b1579f43c5f88783be744d20f9df48567471002d50d7fbbe9a84f2`  
		Last Modified: Tue, 01 Sep 2020 00:32:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd0245d0ee5de14ac31465b43d4761e2c6b5f6554ac131d5c69e9a62b8b7943`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c9ca872243ac437ea220397f5ade201b20e5178214c4e59bbe24a645c02f2`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 7.9 MB (7928853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6138db20f867446ba731c89d1a122c6ea3ccf094213787d187d7cbaccb0c7d8`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 3.0 MB (3023127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f77e821260917b4fa3691d6e4cfda019adea678ca24d055ad067fdc8d95010`  
		Last Modified: Tue, 01 Sep 2020 05:08:25 GMT  
		Size: 184.2 MB (184238858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b673d07c9cd6d327d5134faf2f3b468b126165d6ff3611f980a2149d9b616daf`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b66f8f62ca9ea0f3ec85970e8c4e9c8191604779bbb51b338e322ad549f5a`  
		Last Modified: Tue, 01 Sep 2020 05:07:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:01fa1857b3cf6d870b3f80925838fc70f395e3f94905ecb4c4104ef9c51f331d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325308985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ece7e8752b036774e20a6feed00e4ff41063a283273fc0760aead8f655d060`
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
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
# Fri, 07 Aug 2020 08:25:17 GMT
WORKDIR /src
# Fri, 07 Aug 2020 08:25:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 08:25:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 08:25:23 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 08:25:24 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 08:26:43 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 08:26:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 08:26:51 GMT
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
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c975007342c2ccf0fd2ec1231bbcf2febae5b46c5a18d3261d8066877bdd8`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e900c935258ea5860f9187b513d6fecd815740acc9e33528a9faf0be361d462a`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 7.1 MB (7144924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8990e9c17542b59ea63a50f939defa16c902442ca269c398725eee23674c1e2a`  
		Last Modified: Fri, 07 Aug 2020 08:27:12 GMT  
		Size: 3.0 MB (3019055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa76292e48dfea062acf29eee1e371d5d21420ea90a3c7ffffd631e9c9ff18`  
		Last Modified: Fri, 07 Aug 2020 08:28:04 GMT  
		Size: 184.2 MB (184242015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38253d5b437341664ed152f62f4f0ce8ce5ecdea13fbfda26444b1c0e9ed5dab`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97293801893b82e8a489a88fef714238eb6fb8b1f07ced09ed6764b4147dc6c5`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:124065dc5beb43579f37a540a8930aecd5ebf3d02cd0ae68167bc8824520f77b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325660846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3453b4b2e689e79f1907b074f5c4603a23f987cf307affb274fc1d77e124951f`
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
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
# Fri, 07 Aug 2020 05:58:27 GMT
WORKDIR /src
# Fri, 07 Aug 2020 05:58:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 05:58:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 05:58:35 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 05:58:36 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 05:59:04 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 05:59:09 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 05:59:10 GMT
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
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c598e861ee2e75ef77b4b11f54826ea9db3b637e319ec773f172bae728861be`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5def1e917e01e170f23824bbb783a3982802762418cc48bc2979138d907a96f4`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 8.5 MB (8499915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2c64f3790a0d43891765daae1a55e7ac9dad5c9c7138ddc043ee8f2e080832`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 3.0 MB (3019053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84659d7cd43bedfe10c7a63b22774321083e39b3d60273f726d1ea66ba786ed`  
		Last Modified: Fri, 07 Aug 2020 06:00:07 GMT  
		Size: 184.2 MB (184235645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11d419d5c18b2261c6d45db835f5da794372b6e5a36d9a7f27c3c793dc93df6`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af95d24524d8beb60b236e5c6bcfe19e617bc70767145f2986274c17fed4806`  
		Last Modified: Fri, 07 Aug 2020 05:59:29 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ce1d72f2e1c9f99984f4152d6c1acb304da507da6fc8d3af2d03c25c556ddfe0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324934001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232082dc319bce4f2e67e7efd0cb0933060415808b2fc41475fd4faaf57f054`
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
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
# Fri, 07 Aug 2020 07:38:01 GMT
WORKDIR /src
# Fri, 07 Aug 2020 07:38:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 07:38:16 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 07:38:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 07:38:35 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 07:43:22 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 07:43:32 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 07:43:37 GMT
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
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23db22a9abc815754f8e1f927f04de04bddcb1afa3ea79d1cea8ddef59394a`  
		Last Modified: Fri, 07 Aug 2020 07:43:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6946784ea4945b4bb7a1e6a741e6ae57adeec2912fa477210d9f788e29e7b6c1`  
		Last Modified: Fri, 07 Aug 2020 07:43:56 GMT  
		Size: 8.9 MB (8920010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86177595574ec70181b38420a8c59d367d388bbda0aaf6599c16ab2949430a72`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 3.0 MB (3019596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2029c5d6ea2b7ec4288a32178cea6f0c98c7d4ab9436b78276764a9d654b26e`  
		Last Modified: Fri, 07 Aug 2020 07:44:21 GMT  
		Size: 184.2 MB (184243881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc6284fd669b9914e6857ebda50250d4cab3add6cf36b1ca4554dcc3f0451e`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b7863551d486cc29a789a99d0da68c42c43420212638902e754f4a820c6df0`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-builder` - linux; s390x

```console
$ docker pull caddy@sha256:50b240ca3aee2cb5bce75f9e3c9fd8d2bd05e11512068b589b8d7e781ef2f7bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305647488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eaea38df2e6f50d082a147dff19a1aaa3ad1753739d5fea6760f553cc597422`
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
# Mon, 31 Aug 2020 23:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Mon, 31 Aug 2020 23:59:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Mon, 31 Aug 2020 23:59:15 GMT
ENV GOPATH=/go
# Mon, 31 Aug 2020 23:59:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 31 Aug 2020 23:59:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 31 Aug 2020 23:59:19 GMT
WORKDIR /go
# Tue, 01 Sep 2020 07:37:18 GMT
WORKDIR /src
# Tue, 01 Sep 2020 07:37:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 07:37:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 07:37:22 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 07:37:22 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 07:37:43 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 07:37:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 07:37:52 GMT
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
	-	`sha256:a2005a360724d6d0eb9cecb55f41da04ca8b3400aa7f88d7ff11e9835fb72922`  
		Last Modified: Tue, 01 Sep 2020 00:04:45 GMT  
		Size: 107.2 MB (107190262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b4c4693d4739d62931fa7ec3620a508a792b809822f1f54ef41ae22737ca1b`  
		Last Modified: Tue, 01 Sep 2020 00:04:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6855ec6d51582da654fc233916c0c62aeeddebbccae4174193309eebdc19e559`  
		Last Modified: Tue, 01 Sep 2020 07:38:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edab9907cc22491b00ad7b15c11201e564279a4430ae9892f214b5dc1674056d`  
		Last Modified: Tue, 01 Sep 2020 07:38:06 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457266992ddbe120862122b8d15c05407a03176a13559eebba7a5287e9620cd6`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 3.0 MB (3023067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78e05b7af46d802e3327061221d58c7234a42d6580c91d6a3477874af8ebba`  
		Last Modified: Tue, 01 Sep 2020 07:38:21 GMT  
		Size: 184.2 MB (184231451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a138fc0b86c651c89f60bb30e36865ebbc81ef4ddbffc515c5d3d2781b25`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45315269c7b47f3bb075e8458a30d6a9c06b8872d855535eb3d38f45bb533df`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore`

```console
$ docker pull caddy@sha256:721776712ea5abbd5baef79a760bc7d1ee00e50d6f45e619eb642aec031b5305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

### `caddy:2.1.1-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.1.1-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c11b198f695a66e3690d752dd7dc202e03e06d4804d8aec6f953d1edbbe7c23b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `caddy:2.1.1-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.1.1-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6d37c022d1fcc3cddcf61c53ac3c4b5d6a1f1af4de9e91dfc799d6c2c26f608a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `caddy:2.1.1-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull caddy@sha256:414a95b02fe627ddb1c5644f51b1cdcfc75cfdded416424005e307e834d5f086
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
$ docker pull caddy@sha256:0fc57db9e46d2a71ee3903d22b5ce41e96cdc7a4f17f1c60f654a752b7299a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331162586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48efad8af5ceb779c7ff2fe387448d1d710ffc33d9b3f9abc95d885cd1f64b47`
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
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
# Fri, 07 Aug 2020 03:13:30 GMT
WORKDIR /src
# Fri, 07 Aug 2020 03:13:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 03:13:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 03:13:33 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 03:13:34 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 03:13:49 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 03:13:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 03:13:50 GMT
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
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fe5626f0254b9f60f5f61a291f5046b02ccfbc3f7081b0a44dddbca1397d`  
		Last Modified: Fri, 07 Aug 2020 03:14:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f972bf098f3488dd8a94d2eae2bcb6fc7a10b36175bcccca81baeb51fba4e9`  
		Last Modified: Fri, 07 Aug 2020 03:14:03 GMT  
		Size: 8.3 MB (8310028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bcf269b3e113e083f6a305bff186764723167a9b9625f602894d9cdd105c9a`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 3.0 MB (3022872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe8c223c437ec7b5d6ac8dfce77a26db0a34330288c7d0dbe3081116fe63db`  
		Last Modified: Fri, 07 Aug 2020 03:14:28 GMT  
		Size: 184.2 MB (184231010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35266c5be392980f82d35b0575940e3625d38bd55e3c03ca95e9dbd254b875eb`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb543dcf1b950699168feb583f397202802260bd84ef2c230f752539701b30fd`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:982248ee8c889b1765b1481b67ed5d16180a4ff6e82616d8dc82d56484a99742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.7 MB (301748871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eaed8f6193bdd4f5d28ddfbac079c84ae0260c92d2d9dd4016e87240089423d`
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
# Mon, 31 Aug 2020 23:55:22 GMT
ENV GOLANG_VERSION=1.14.7
# Tue, 01 Sep 2020 00:03:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 01 Sep 2020 00:03:34 GMT
ENV GOPATH=/go
# Tue, 01 Sep 2020 00:03:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Sep 2020 00:03:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Sep 2020 00:03:40 GMT
WORKDIR /go
# Tue, 01 Sep 2020 05:03:15 GMT
WORKDIR /src
# Tue, 01 Sep 2020 05:03:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 05:03:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 05:04:40 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 05:04:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 05:06:45 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 05:07:00 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 05:07:07 GMT
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
	-	`sha256:d80d870b4111d9793e4a962df54668501236ab71f0b3bd501fe19d8832d95bd2`  
		Last Modified: Tue, 01 Sep 2020 00:33:29 GMT  
		Size: 103.7 MB (103670838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbe42781b1579f43c5f88783be744d20f9df48567471002d50d7fbbe9a84f2`  
		Last Modified: Tue, 01 Sep 2020 00:32:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd0245d0ee5de14ac31465b43d4761e2c6b5f6554ac131d5c69e9a62b8b7943`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c9ca872243ac437ea220397f5ade201b20e5178214c4e59bbe24a645c02f2`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 7.9 MB (7928853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6138db20f867446ba731c89d1a122c6ea3ccf094213787d187d7cbaccb0c7d8`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 3.0 MB (3023127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f77e821260917b4fa3691d6e4cfda019adea678ca24d055ad067fdc8d95010`  
		Last Modified: Tue, 01 Sep 2020 05:08:25 GMT  
		Size: 184.2 MB (184238858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b673d07c9cd6d327d5134faf2f3b468b126165d6ff3611f980a2149d9b616daf`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b66f8f62ca9ea0f3ec85970e8c4e9c8191604779bbb51b338e322ad549f5a`  
		Last Modified: Tue, 01 Sep 2020 05:07:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:01fa1857b3cf6d870b3f80925838fc70f395e3f94905ecb4c4104ef9c51f331d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325308985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ece7e8752b036774e20a6feed00e4ff41063a283273fc0760aead8f655d060`
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
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
# Fri, 07 Aug 2020 08:25:17 GMT
WORKDIR /src
# Fri, 07 Aug 2020 08:25:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 08:25:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 08:25:23 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 08:25:24 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 08:26:43 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 08:26:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 08:26:51 GMT
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
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c975007342c2ccf0fd2ec1231bbcf2febae5b46c5a18d3261d8066877bdd8`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e900c935258ea5860f9187b513d6fecd815740acc9e33528a9faf0be361d462a`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 7.1 MB (7144924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8990e9c17542b59ea63a50f939defa16c902442ca269c398725eee23674c1e2a`  
		Last Modified: Fri, 07 Aug 2020 08:27:12 GMT  
		Size: 3.0 MB (3019055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa76292e48dfea062acf29eee1e371d5d21420ea90a3c7ffffd631e9c9ff18`  
		Last Modified: Fri, 07 Aug 2020 08:28:04 GMT  
		Size: 184.2 MB (184242015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38253d5b437341664ed152f62f4f0ce8ce5ecdea13fbfda26444b1c0e9ed5dab`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97293801893b82e8a489a88fef714238eb6fb8b1f07ced09ed6764b4147dc6c5`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:124065dc5beb43579f37a540a8930aecd5ebf3d02cd0ae68167bc8824520f77b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325660846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3453b4b2e689e79f1907b074f5c4603a23f987cf307affb274fc1d77e124951f`
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
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
# Fri, 07 Aug 2020 05:58:27 GMT
WORKDIR /src
# Fri, 07 Aug 2020 05:58:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 05:58:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 05:58:35 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 05:58:36 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 05:59:04 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 05:59:09 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 05:59:10 GMT
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
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c598e861ee2e75ef77b4b11f54826ea9db3b637e319ec773f172bae728861be`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5def1e917e01e170f23824bbb783a3982802762418cc48bc2979138d907a96f4`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 8.5 MB (8499915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2c64f3790a0d43891765daae1a55e7ac9dad5c9c7138ddc043ee8f2e080832`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 3.0 MB (3019053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84659d7cd43bedfe10c7a63b22774321083e39b3d60273f726d1ea66ba786ed`  
		Last Modified: Fri, 07 Aug 2020 06:00:07 GMT  
		Size: 184.2 MB (184235645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11d419d5c18b2261c6d45db835f5da794372b6e5a36d9a7f27c3c793dc93df6`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af95d24524d8beb60b236e5c6bcfe19e617bc70767145f2986274c17fed4806`  
		Last Modified: Fri, 07 Aug 2020 05:59:29 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ce1d72f2e1c9f99984f4152d6c1acb304da507da6fc8d3af2d03c25c556ddfe0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324934001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232082dc319bce4f2e67e7efd0cb0933060415808b2fc41475fd4faaf57f054`
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
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
# Fri, 07 Aug 2020 07:38:01 GMT
WORKDIR /src
# Fri, 07 Aug 2020 07:38:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 07:38:16 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 07:38:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 07:38:35 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 07:43:22 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 07:43:32 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 07:43:37 GMT
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
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23db22a9abc815754f8e1f927f04de04bddcb1afa3ea79d1cea8ddef59394a`  
		Last Modified: Fri, 07 Aug 2020 07:43:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6946784ea4945b4bb7a1e6a741e6ae57adeec2912fa477210d9f788e29e7b6c1`  
		Last Modified: Fri, 07 Aug 2020 07:43:56 GMT  
		Size: 8.9 MB (8920010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86177595574ec70181b38420a8c59d367d388bbda0aaf6599c16ab2949430a72`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 3.0 MB (3019596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2029c5d6ea2b7ec4288a32178cea6f0c98c7d4ab9436b78276764a9d654b26e`  
		Last Modified: Fri, 07 Aug 2020 07:44:21 GMT  
		Size: 184.2 MB (184243881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc6284fd669b9914e6857ebda50250d4cab3add6cf36b1ca4554dcc3f0451e`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b7863551d486cc29a789a99d0da68c42c43420212638902e754f4a820c6df0`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:50b240ca3aee2cb5bce75f9e3c9fd8d2bd05e11512068b589b8d7e781ef2f7bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305647488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eaea38df2e6f50d082a147dff19a1aaa3ad1753739d5fea6760f553cc597422`
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
# Mon, 31 Aug 2020 23:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Mon, 31 Aug 2020 23:59:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Mon, 31 Aug 2020 23:59:15 GMT
ENV GOPATH=/go
# Mon, 31 Aug 2020 23:59:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 31 Aug 2020 23:59:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 31 Aug 2020 23:59:19 GMT
WORKDIR /go
# Tue, 01 Sep 2020 07:37:18 GMT
WORKDIR /src
# Tue, 01 Sep 2020 07:37:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 07:37:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 07:37:22 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 07:37:22 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 07:37:43 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 07:37:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 07:37:52 GMT
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
	-	`sha256:a2005a360724d6d0eb9cecb55f41da04ca8b3400aa7f88d7ff11e9835fb72922`  
		Last Modified: Tue, 01 Sep 2020 00:04:45 GMT  
		Size: 107.2 MB (107190262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b4c4693d4739d62931fa7ec3620a508a792b809822f1f54ef41ae22737ca1b`  
		Last Modified: Tue, 01 Sep 2020 00:04:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6855ec6d51582da654fc233916c0c62aeeddebbccae4174193309eebdc19e559`  
		Last Modified: Tue, 01 Sep 2020 07:38:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edab9907cc22491b00ad7b15c11201e564279a4430ae9892f214b5dc1674056d`  
		Last Modified: Tue, 01 Sep 2020 07:38:06 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457266992ddbe120862122b8d15c05407a03176a13559eebba7a5287e9620cd6`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 3.0 MB (3023067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78e05b7af46d802e3327061221d58c7234a42d6580c91d6a3477874af8ebba`  
		Last Modified: Tue, 01 Sep 2020 07:38:21 GMT  
		Size: 184.2 MB (184231451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a138fc0b86c651c89f60bb30e36865ebbc81ef4ddbffc515c5d3d2781b25`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45315269c7b47f3bb075e8458a30d6a9c06b8872d855535eb3d38f45bb533df`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:721776712ea5abbd5baef79a760bc7d1ee00e50d6f45e619eb642aec031b5305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c11b198f695a66e3690d752dd7dc202e03e06d4804d8aec6f953d1edbbe7c23b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6d37c022d1fcc3cddcf61c53ac3c4b5d6a1f1af4de9e91dfc799d6c2c26f608a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
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
$ docker pull caddy@sha256:414a95b02fe627ddb1c5644f51b1cdcfc75cfdded416424005e307e834d5f086
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
$ docker pull caddy@sha256:0fc57db9e46d2a71ee3903d22b5ce41e96cdc7a4f17f1c60f654a752b7299a3e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.2 MB (331162586 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48efad8af5ceb779c7ff2fe387448d1d710ffc33d9b3f9abc95d885cd1f64b47`
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
# Fri, 07 Aug 2020 00:34:36 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 00:39:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 00:39:11 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 00:39:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 00:39:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 00:39:12 GMT
WORKDIR /go
# Fri, 07 Aug 2020 03:13:30 GMT
WORKDIR /src
# Fri, 07 Aug 2020 03:13:32 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 03:13:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 03:13:33 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 03:13:34 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 03:13:49 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 03:13:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 03:13:50 GMT
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
	-	`sha256:f17c8f1adafbac0b972377ff2e912a0364892f70f78c96cfa8e47ebea5e07a7a`  
		Last Modified: Fri, 07 Aug 2020 00:50:52 GMT  
		Size: 132.5 MB (132517497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03954754c53ab5ee0633f746077a6c09ea2b1dcaf9b728d80ded1c608c63af81`  
		Last Modified: Fri, 07 Aug 2020 00:50:25 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71fe5626f0254b9f60f5f61a291f5046b02ccfbc3f7081b0a44dddbca1397d`  
		Last Modified: Fri, 07 Aug 2020 03:14:02 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f972bf098f3488dd8a94d2eae2bcb6fc7a10b36175bcccca81baeb51fba4e9`  
		Last Modified: Fri, 07 Aug 2020 03:14:03 GMT  
		Size: 8.3 MB (8310028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bcf269b3e113e083f6a305bff186764723167a9b9625f602894d9cdd105c9a`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 3.0 MB (3022872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80fe8c223c437ec7b5d6ac8dfce77a26db0a34330288c7d0dbe3081116fe63db`  
		Last Modified: Fri, 07 Aug 2020 03:14:28 GMT  
		Size: 184.2 MB (184231010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35266c5be392980f82d35b0575940e3625d38bd55e3c03ca95e9dbd254b875eb`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 511.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb543dcf1b950699168feb583f397202802260bd84ef2c230f752539701b30fd`  
		Last Modified: Fri, 07 Aug 2020 03:14:01 GMT  
		Size: 151.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:982248ee8c889b1765b1481b67ed5d16180a4ff6e82616d8dc82d56484a99742
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.7 MB (301748871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eaed8f6193bdd4f5d28ddfbac079c84ae0260c92d2d9dd4016e87240089423d`
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
# Mon, 31 Aug 2020 23:55:22 GMT
ENV GOLANG_VERSION=1.14.7
# Tue, 01 Sep 2020 00:03:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Tue, 01 Sep 2020 00:03:34 GMT
ENV GOPATH=/go
# Tue, 01 Sep 2020 00:03:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 01 Sep 2020 00:03:38 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 01 Sep 2020 00:03:40 GMT
WORKDIR /go
# Tue, 01 Sep 2020 05:03:15 GMT
WORKDIR /src
# Tue, 01 Sep 2020 05:03:46 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 05:03:57 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 05:04:40 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 05:04:51 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 05:06:45 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 05:07:00 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 05:07:07 GMT
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
	-	`sha256:d80d870b4111d9793e4a962df54668501236ab71f0b3bd501fe19d8832d95bd2`  
		Last Modified: Tue, 01 Sep 2020 00:33:29 GMT  
		Size: 103.7 MB (103670838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccbe42781b1579f43c5f88783be744d20f9df48567471002d50d7fbbe9a84f2`  
		Last Modified: Tue, 01 Sep 2020 00:32:59 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbd0245d0ee5de14ac31465b43d4761e2c6b5f6554ac131d5c69e9a62b8b7943`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601c9ca872243ac437ea220397f5ade201b20e5178214c4e59bbe24a645c02f2`  
		Last Modified: Tue, 01 Sep 2020 05:07:39 GMT  
		Size: 7.9 MB (7928853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6138db20f867446ba731c89d1a122c6ea3ccf094213787d187d7cbaccb0c7d8`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 3.0 MB (3023127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3f77e821260917b4fa3691d6e4cfda019adea678ca24d055ad067fdc8d95010`  
		Last Modified: Tue, 01 Sep 2020 05:08:25 GMT  
		Size: 184.2 MB (184238858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b673d07c9cd6d327d5134faf2f3b468b126165d6ff3611f980a2149d9b616daf`  
		Last Modified: Tue, 01 Sep 2020 05:07:36 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b66f8f62ca9ea0f3ec85970e8c4e9c8191604779bbb51b338e322ad549f5a`  
		Last Modified: Tue, 01 Sep 2020 05:07:38 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:01fa1857b3cf6d870b3f80925838fc70f395e3f94905ecb4c4104ef9c51f331d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325308985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82ece7e8752b036774e20a6feed00e4ff41063a283273fc0760aead8f655d060`
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
# Fri, 07 Aug 2020 01:20:45 GMT
ENV GOLANG_VERSION=1.14.7
# Fri, 07 Aug 2020 02:19:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Fri, 07 Aug 2020 02:19:26 GMT
ENV GOPATH=/go
# Fri, 07 Aug 2020 02:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 Aug 2020 02:19:41 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 Aug 2020 02:19:48 GMT
WORKDIR /go
# Fri, 07 Aug 2020 08:25:17 GMT
WORKDIR /src
# Fri, 07 Aug 2020 08:25:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 08:25:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 08:25:23 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 08:25:24 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 08:26:43 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 08:26:50 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 08:26:51 GMT
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
	-	`sha256:da757ec41ca8393023f8db623f117071cb05c07ebf47da0f293c91deca9ebb20`  
		Last Modified: Fri, 07 Aug 2020 05:02:34 GMT  
		Size: 128.2 MB (128213206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:692751ab01ad41ed9df38cab0ec15fb400ac55ccebbbac4348dde69682731043`  
		Last Modified: Fri, 07 Aug 2020 05:01:53 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d43c975007342c2ccf0fd2ec1231bbcf2febae5b46c5a18d3261d8066877bdd8`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e900c935258ea5860f9187b513d6fecd815740acc9e33528a9faf0be361d462a`  
		Last Modified: Fri, 07 Aug 2020 08:27:13 GMT  
		Size: 7.1 MB (7144924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8990e9c17542b59ea63a50f939defa16c902442ca269c398725eee23674c1e2a`  
		Last Modified: Fri, 07 Aug 2020 08:27:12 GMT  
		Size: 3.0 MB (3019055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa76292e48dfea062acf29eee1e371d5d21420ea90a3c7ffffd631e9c9ff18`  
		Last Modified: Fri, 07 Aug 2020 08:28:04 GMT  
		Size: 184.2 MB (184242015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38253d5b437341664ed152f62f4f0ce8ce5ecdea13fbfda26444b1c0e9ed5dab`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 512.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97293801893b82e8a489a88fef714238eb6fb8b1f07ced09ed6764b4147dc6c5`  
		Last Modified: Fri, 07 Aug 2020 08:27:11 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:124065dc5beb43579f37a540a8930aecd5ebf3d02cd0ae68167bc8824520f77b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325660846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3453b4b2e689e79f1907b074f5c4603a23f987cf307affb274fc1d77e124951f`
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
# Thu, 06 Aug 2020 23:49:43 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 23:54:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 23:54:14 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 23:54:22 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 23:54:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 23:54:57 GMT
WORKDIR /go
# Fri, 07 Aug 2020 05:58:27 GMT
WORKDIR /src
# Fri, 07 Aug 2020 05:58:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 05:58:32 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 05:58:35 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 05:58:36 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 05:59:04 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 05:59:09 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 05:59:10 GMT
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
	-	`sha256:5f7ac17f646aa1c638cf5ff4a0ba58fc0796273c5fe2026e08fda7f5b99ad69b`  
		Last Modified: Fri, 07 Aug 2020 00:24:56 GMT  
		Size: 126.9 MB (126914145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939e11ed57492a89d0d2dbd813ddbc762da2c5c82e31f0cf4539d62a70240671`  
		Last Modified: Fri, 07 Aug 2020 00:24:18 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c598e861ee2e75ef77b4b11f54826ea9db3b637e319ec773f172bae728861be`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5def1e917e01e170f23824bbb783a3982802762418cc48bc2979138d907a96f4`  
		Last Modified: Fri, 07 Aug 2020 05:59:31 GMT  
		Size: 8.5 MB (8499915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d2c64f3790a0d43891765daae1a55e7ac9dad5c9c7138ddc043ee8f2e080832`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 3.0 MB (3019053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84659d7cd43bedfe10c7a63b22774321083e39b3d60273f726d1ea66ba786ed`  
		Last Modified: Fri, 07 Aug 2020 06:00:07 GMT  
		Size: 184.2 MB (184235645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11d419d5c18b2261c6d45db835f5da794372b6e5a36d9a7f27c3c793dc93df6`  
		Last Modified: Fri, 07 Aug 2020 05:59:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af95d24524d8beb60b236e5c6bcfe19e617bc70767145f2986274c17fed4806`  
		Last Modified: Fri, 07 Aug 2020 05:59:29 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:ce1d72f2e1c9f99984f4152d6c1acb304da507da6fc8d3af2d03c25c556ddfe0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.9 MB (324934001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4232082dc319bce4f2e67e7efd0cb0933060415808b2fc41475fd4faaf57f054`
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
# Thu, 06 Aug 2020 22:54:28 GMT
ENV GOLANG_VERSION=1.14.7
# Thu, 06 Aug 2020 22:57:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		musl-dev 		openssl 		go 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		wget -O go.tgz "https://golang.org/dl/go$GOLANG_VERSION.src.tar.gz"; 	echo '064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3 *go.tgz' | sha256sum -c -; 	tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		cd /usr/local/go/src; 	./make.bash; 		rm -rf 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 	; 	apk del .build-deps; 		export PATH="/usr/local/go/bin:$PATH"; 	go version
# Thu, 06 Aug 2020 22:57:38 GMT
ENV GOPATH=/go
# Thu, 06 Aug 2020 22:57:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 Aug 2020 22:58:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 Aug 2020 22:58:31 GMT
WORKDIR /go
# Fri, 07 Aug 2020 07:38:01 GMT
WORKDIR /src
# Fri, 07 Aug 2020 07:38:12 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 Aug 2020 07:38:16 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Fri, 07 Aug 2020 07:38:29 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Fri, 07 Aug 2020 07:38:35 GMT
WORKDIR /src/caddy/cmd/caddy
# Fri, 07 Aug 2020 07:43:22 GMT
RUN go get -d ./...
# Fri, 07 Aug 2020 07:43:32 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Fri, 07 Aug 2020 07:43:37 GMT
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
	-	`sha256:ae0064c9a2ae1e51dfb1cf3cc1d24a7946656a17fa59dccd07879e4c0531e8cc`  
		Last Modified: Thu, 06 Aug 2020 23:13:59 GMT  
		Size: 125.7 MB (125659150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6663dc31955b59f1c4a3fd5a651c54694b4e1ae7124b6ed3ed11713a1136213`  
		Last Modified: Thu, 06 Aug 2020 23:13:32 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe23db22a9abc815754f8e1f927f04de04bddcb1afa3ea79d1cea8ddef59394a`  
		Last Modified: Fri, 07 Aug 2020 07:43:57 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6946784ea4945b4bb7a1e6a741e6ae57adeec2912fa477210d9f788e29e7b6c1`  
		Last Modified: Fri, 07 Aug 2020 07:43:56 GMT  
		Size: 8.9 MB (8920010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86177595574ec70181b38420a8c59d367d388bbda0aaf6599c16ab2949430a72`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 3.0 MB (3019596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2029c5d6ea2b7ec4288a32178cea6f0c98c7d4ab9436b78276764a9d654b26e`  
		Last Modified: Fri, 07 Aug 2020 07:44:21 GMT  
		Size: 184.2 MB (184243881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fbc6284fd669b9914e6857ebda50250d4cab3add6cf36b1ca4554dcc3f0451e`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b7863551d486cc29a789a99d0da68c42c43420212638902e754f4a820c6df0`  
		Last Modified: Fri, 07 Aug 2020 07:43:54 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:50b240ca3aee2cb5bce75f9e3c9fd8d2bd05e11512068b589b8d7e781ef2f7bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.6 MB (305647488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0eaea38df2e6f50d082a147dff19a1aaa3ad1753739d5fea6760f553cc597422`
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
# Mon, 31 Aug 2020 23:56:35 GMT
ENV GOLANG_VERSION=1.14.7
# Mon, 31 Aug 2020 23:59:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	export 		GOROOT_BOOTSTRAP="$(go env GOROOT)" 		GOOS="$(go env GOOS)" 		GOARCH="$(go env GOARCH)" 		GOHOSTOS="$(go env GOHOSTOS)" 		GOHOSTARCH="$(go env GOHOSTARCH)" 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		armhf) export GOARM='6' ;; 		armv7) export GOARM='7' ;; 		x86) export GO386='387' ;; 	esac; 		url='https://storage.googleapis.com/golang/go1.14.7.src.tar.gz'; 	sha256='064392433563660c73186991c0a315787688e7c38a561e26647686f89b6c30e3'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		goEnv="$(go env | sed -rn -e '/^GO(OS|ARCH|ARM|386)=/s//export \0/p')"; 	eval "$goEnv"; 	[ -n "$GOOS" ]; 	[ -n "$GOARCH" ]; 	( 		cd /usr/local/go/src; 		./make.bash; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Mon, 31 Aug 2020 23:59:15 GMT
ENV GOPATH=/go
# Mon, 31 Aug 2020 23:59:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 31 Aug 2020 23:59:18 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 31 Aug 2020 23:59:19 GMT
WORKDIR /go
# Tue, 01 Sep 2020 07:37:18 GMT
WORKDIR /src
# Tue, 01 Sep 2020 07:37:20 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 01 Sep 2020 07:37:20 GMT
ENV CADDY_SOURCE_VERSION=v2.1.1
# Tue, 01 Sep 2020 07:37:22 GMT
RUN git clone -b $CADDY_SOURCE_VERSION https://github.com/caddyserver/caddy.git --single-branch
# Tue, 01 Sep 2020 07:37:22 GMT
WORKDIR /src/caddy/cmd/caddy
# Tue, 01 Sep 2020 07:37:43 GMT
RUN go get -d ./...
# Tue, 01 Sep 2020 07:37:52 GMT
COPY file:ed649bfc3baea8b334bfe88e6442632ecdc59b7c07d01b02a6c4558e5d77f98a in /usr/bin/caddy-builder 
# Tue, 01 Sep 2020 07:37:52 GMT
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
	-	`sha256:a2005a360724d6d0eb9cecb55f41da04ca8b3400aa7f88d7ff11e9835fb72922`  
		Last Modified: Tue, 01 Sep 2020 00:04:45 GMT  
		Size: 107.2 MB (107190262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b4c4693d4739d62931fa7ec3620a508a792b809822f1f54ef41ae22737ca1b`  
		Last Modified: Tue, 01 Sep 2020 00:04:23 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6855ec6d51582da654fc233916c0c62aeeddebbccae4174193309eebdc19e559`  
		Last Modified: Tue, 01 Sep 2020 07:38:07 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edab9907cc22491b00ad7b15c11201e564279a4430ae9892f214b5dc1674056d`  
		Last Modified: Tue, 01 Sep 2020 07:38:06 GMT  
		Size: 8.4 MB (8352247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457266992ddbe120862122b8d15c05407a03176a13559eebba7a5287e9620cd6`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 3.0 MB (3023067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c78e05b7af46d802e3327061221d58c7234a42d6580c91d6a3477874af8ebba`  
		Last Modified: Tue, 01 Sep 2020 07:38:21 GMT  
		Size: 184.2 MB (184231451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a51a138fc0b86c651c89f60bb30e36865ebbc81ef4ddbffc515c5d3d2781b25`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45315269c7b47f3bb075e8458a30d6a9c06b8872d855535eb3d38f45bb533df`  
		Last Modified: Tue, 01 Sep 2020 07:38:05 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:76e5b24fe40ee203c6da262f5d5a2661fcc4b7c49ad0e2c13d10bd40a70af476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

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

### `caddy:latest` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:721776712ea5abbd5baef79a760bc7d1ee00e50d6f45e619eb642aec031b5305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64
	-	windows version 10.0.14393.3866; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:c11b198f695a66e3690d752dd7dc202e03e06d4804d8aec6f953d1edbbe7c23b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1397; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1397; amd64

```console
$ docker pull caddy@sha256:6fe7722afe7f2a04904666b05e8b95bacc3ace24dc70c232c3da08a456a5eb4e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2363011231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f2edf58a1b9a89ae4c32c405481fbdadf112e71860ce5ae3289e300961996bc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 06 Aug 2020 16:53:49 GMT
RUN Install update 1809-amd64
# Tue, 11 Aug 2020 20:36:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:20:12 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:20:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:20:52 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:21:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:21:26 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:21:27 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:21:28 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:21:29 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:21:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:21:31 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:21:32 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:21:33 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:21:34 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:21:35 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:21:35 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:21:36 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:21:37 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:21:53 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:21:54 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3ab49687905cb6183025d5ec648fe62fb3d7039a9cf1fe09ef94a62d89d219db`  
		Size: 617.5 MB (617534122 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43065500f09f35124a5d71517aa493fd23ad75660682600f7f6b40aa7629ac78`  
		Last Modified: Tue, 11 Aug 2020 20:54:54 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee0c1b06dd703a6d5247afb68291748c99b4f9de1c9e2ae9e90b6115b87117a`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c2c051346b0f0aef066e3b4ad72a01809f8403d1021122c7ad6c80579624d9`  
		Last Modified: Wed, 12 Aug 2020 18:26:38 GMT  
		Size: 9.2 MB (9156082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4a07e46ea2519a094a5803c355dad838f87a366d6743b5f08594933603918e6`  
		Last Modified: Wed, 12 Aug 2020 18:26:35 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54bec25576d66f070dadca03df4f2326052c693797df2cf7cf08f802ea4ab629`  
		Last Modified: Wed, 12 Aug 2020 18:26:46 GMT  
		Size: 17.7 MB (17676360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9439354479a9b9ea242f62263aa94dee60053ab3adb58d309d98e64b44fc0016`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16291dc3e63bda8ff560d924dc41414b9dc32bad594914bc6ab097c2a948781`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedab8476a2860f0d7de59a0b4f06b6eaf1f3ded4ff5790d1b3f5a4b4cbc6bcb`  
		Last Modified: Wed, 12 Aug 2020 18:26:32 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8649d8c083bd21fda11da6f2529e851f3b287690ee965e0998941fec946fd5`  
		Last Modified: Wed, 12 Aug 2020 18:26:33 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faddf1f4f68667d81626e152e392a3d61cdc83170e14ff63d891d3941b38ed9`  
		Last Modified: Wed, 12 Aug 2020 18:26:31 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30332dcef86cb8c8e6f3245d12535df0ebf06190116bb6348465cf6912bfb554`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f5b14ecf0c1f35c6670fa00efbbcc272a38e1416f3acc8b160e51dc6e115cb`  
		Last Modified: Wed, 12 Aug 2020 18:26:30 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191f0f12602e0731b99f83f0398d369d0873f08ad3d082f80b19ddeb8257f2e7`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d883df69b591966b718187d2d291242be743bd4fead8120733ac08479b0f13b3`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4150978f9389a2ebf8b36a8e2ba95ab279748935ee59a5391387a140f9213371`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa221c48f90ca5f19482982a18f17d06c5ee39094c7f1834c6dd56bb335d0e83`  
		Last Modified: Wed, 12 Aug 2020 18:26:28 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74fccce77db6e74ca68b1979012aee5727734baad68fe9c05261cb24d7dcb71`  
		Last Modified: Wed, 12 Aug 2020 18:26:27 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d040f084082fb82dc8d77d688563c38c86c7ced0e30f81491b5ef6930a618e9e`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0150e9e30dbce51e16baa13a2cfdf8f8c357bf83402bd5efc9261b6c1cca2c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4964b178be4f0bf5b7acbc0571d22fdaf33dacf0dbf6018c3aaea694b66779c`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a67939412cb526125d5df3254e959808d9f0a8a3dea02cb75d122f60f18b0ac`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 290.2 KB (290230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e0a69b1373af956fc482a92110fc6b9d21ce160e6e802f33c3ed5e5c998c27`  
		Last Modified: Wed, 12 Aug 2020 18:26:25 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:6d37c022d1fcc3cddcf61c53ac3c4b5d6a1f1af4de9e91dfc799d6c2c26f608a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3866; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.3866; amd64

```console
$ docker pull caddy@sha256:2e72d4c6fad10d389ee9269c3afb2c59e086bdff525f75b20d54f5955c54f83a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5771148566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5911145356d44266e7c91c58c32736a59af78e56944c17913ce02544739e62fd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 05 Aug 2020 13:27:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 11 Aug 2020 20:31:19 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Aug 2020 18:22:08 GMT
ENV CADDY_DIST_COMMIT=1ae255dd910fe0ad14aeec27eabe4f526bf423ab
# Wed, 12 Aug 2020 18:23:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/$env:CADDY_DIST_COMMIT/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Aug 2020 18:23:28 GMT
ENV CADDY_VERSION=v2.1.1
# Wed, 12 Aug 2020 18:24:51 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.1.1/caddy_2.1.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('435c881bf3d149da2339fdca28cf4bedcba79a3ed6bbd79365113e7e78bd110f544a13ab4976529cf73d4760c64991abed7b6f952ace4396ff5a78d98fcf3e19')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Aug 2020 18:24:53 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Aug 2020 18:24:54 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Aug 2020 18:24:55 GMT
VOLUME [c:/config]
# Wed, 12 Aug 2020 18:24:56 GMT
VOLUME [c:/data]
# Wed, 12 Aug 2020 18:24:57 GMT
LABEL org.opencontainers.image.version=v2.1.1
# Wed, 12 Aug 2020 18:24:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Aug 2020 18:24:59 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Aug 2020 18:25:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Aug 2020 18:25:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Aug 2020 18:25:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Aug 2020 18:25:03 GMT
EXPOSE 80
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 443
# Wed, 12 Aug 2020 18:25:04 GMT
EXPOSE 2019
# Wed, 12 Aug 2020 18:25:47 GMT
RUN caddy version
# Wed, 12 Aug 2020 18:25:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b2151f69990007e1df0a2a0a68997c72a9ce7546d653d17a482a51cc3323c047`  
		Size: 1.7 GB (1668161535 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:32838d9637dc39d4acee78700b0f93d6c8c9d2db755f12c8009c1b51687d3fbd`  
		Last Modified: Tue, 11 Aug 2020 20:54:28 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b43a86f007ceca8251e384223d65f32931f84f5eaab12f53e7aa26d516a017b3`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 1.1 KB (1132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af9c5d103ff70248238b4264ec049dbdeeb49fb8c6ebd2f3ac67e87ee0c2ccad`  
		Last Modified: Wed, 12 Aug 2020 18:27:15 GMT  
		Size: 9.9 MB (9885669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fb79de83d5704b382045fdca2eae660b0e6a785ca2e3430dfd1133e0e9122`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2693981b98fcce2e17fc0b4bf3f20cb5967a773969303ab342383be6740739a3`  
		Last Modified: Wed, 12 Aug 2020 18:27:18 GMT  
		Size: 22.9 MB (22854209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b034aa5ed985b9516ddf63ec579597e71ca87b3abbd520aa9b97ab2be96dc47`  
		Last Modified: Wed, 12 Aug 2020 18:27:11 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2109a5f31d92a8711132ded43517c75a955ce39c775240d1c57521798117e7e`  
		Last Modified: Wed, 12 Aug 2020 18:27:10 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fff09751cabb85773ed00a407970132d5ebb804fb8e582c7e568d159f00e42`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca3f5fd2aa85425fe8a61f1588e9c8e8e81636f61c5d958e50a44ede3b9370d`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808cbe3437a1a12f04ac41855557ca1d69d7ee7fd33a3f235109599166a83996`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ef36d78825131d8e347fcaacfa951d026b1a6ba22f5ba1ed6901ec8092d4f`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f28801f98ff78ea7fc378ac7b7a0368e183ad612050def5c78e9642a6378399`  
		Last Modified: Wed, 12 Aug 2020 18:27:08 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a88279510d22b36b9eeb40fff3bd12114dc2f6b9f4833f88d9c97d93835c55c8`  
		Last Modified: Wed, 12 Aug 2020 18:27:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7d56735e63ef7963447f7aa0bd49914d031c399e1fabb9262c87e8cf4d9fa8`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6047705d42f4a7a216a4d1cb3e2083b895874cedbd1ae40e6eb2c7008c6fc684`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32ac73604d42daeaf8c539a5cb80ffbc7f8e3a7e82897d97869d50e1a0bf420`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a33651212c65fcca362e652e1b0f8dae59bccd9b6a2e67c6b6a1de274f075a21`  
		Last Modified: Wed, 12 Aug 2020 18:27:05 GMT  
		Size: 1.1 KB (1100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c29359fbbdbd6c36070f1d4bff445df9e41117fa0d77e023401e11bee1763f`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca98bb596b991bdab98937fa187545269ab725c7f6930fcea9ca191e30f9c3f`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7789a12a5d8f91e9b2a5e0ce0821192e0ad6977159a96f4f21d54dd5bbc132db`  
		Last Modified: Wed, 12 Aug 2020 18:27:02 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602852425a5a34a59c885f93d92cbc027a26dc3dbd7f00c9522c99036c8268f5`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 239.7 KB (239658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3f8533a57e3bbd15a96c7a518b4c975c8bd3bfaec7ad49eb42e2fffcae0692`  
		Last Modified: Wed, 12 Aug 2020 18:27:03 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
