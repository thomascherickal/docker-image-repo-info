<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2.3.0`](#caddy230)
-	[`caddy:2.3.0-alpine`](#caddy230-alpine)
-	[`caddy:2.3.0-builder`](#caddy230-builder)
-	[`caddy:2.3.0-builder-alpine`](#caddy230-builder-alpine)
-	[`caddy:2.3.0-builder-windowsservercore-1809`](#caddy230-builder-windowsservercore-1809)
-	[`caddy:2.3.0-builder-windowsservercore-ltsc2016`](#caddy230-builder-windowsservercore-ltsc2016)
-	[`caddy:2.3.0-windowsservercore`](#caddy230-windowsservercore)
-	[`caddy:2.3.0-windowsservercore-1809`](#caddy230-windowsservercore-1809)
-	[`caddy:2.3.0-windowsservercore-ltsc2016`](#caddy230-windowsservercore-ltsc2016)
-	[`caddy:2.4.0`](#caddy240)
-	[`caddy:2.4.0-alpine`](#caddy240-alpine)
-	[`caddy:2.4.0-builder`](#caddy240-builder)
-	[`caddy:2.4.0-builder-alpine`](#caddy240-builder-alpine)
-	[`caddy:2.4.0-builder-windowsservercore-1809`](#caddy240-builder-windowsservercore-1809)
-	[`caddy:2.4.0-builder-windowsservercore-ltsc2016`](#caddy240-builder-windowsservercore-ltsc2016)
-	[`caddy:2.4.0-windowsservercore`](#caddy240-windowsservercore)
-	[`caddy:2.4.0-windowsservercore-1809`](#caddy240-windowsservercore-1809)
-	[`caddy:2.4.0-windowsservercore-ltsc2016`](#caddy240-windowsservercore-ltsc2016)
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
$ docker pull caddy@sha256:22f138ef9ab7e91e06e93e0a50de4cbddfa8519e6a3aeaa7abd09bb098996a6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0`

```console
$ docker pull caddy@sha256:c2fa00de2b6926cb006a698038807604a5120113aba713da7be0116598deab13
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0` - linux; amd64

```console
$ docker pull caddy@sha256:6fbf52298c46c55c572670b5395ecaee5d399338003c9bb4e4abed875c542f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7395cc3713b2ca5574a9b4aafc468a1533d16582efe47dcab74ed547540d698a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:10:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:10:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:10:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:10:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:10:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:10:53 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:10:54 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:10:55 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:10:56 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:10:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a0cd9cca5be9b30bbc70611052d1456502e1f338ce4b14946233b21cd6a9a`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 300.0 KB (300016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5666523658a43fbbdff6b8fca498a988f4dcecc3ce027f1701414658c21d4ea`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b097228407f13a161f68b188b0a4f255855b64d84e7b076745a744d5aa7ed8cf`  
		Last Modified: Wed, 14 Apr 2021 20:11:49 GMT  
		Size: 11.6 MB (11622383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40682d93cc09b4592a1b9c08d48d0a956b5eef4f123d80d1a12942482edb6aab`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0df9df9725cab39fe073887c98b54bf7bf1c96b3ed0e23916737c7c4877576c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13856181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce1c33ce4509195edc1c67d2dcd15c6c5fc0b35cec2e90714ec3007739600eb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:45:19 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 19:45:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 19:45:36 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:45:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:46:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:46:04 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:46:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:46:07 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:46:08 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:46:10 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:46:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:46:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:46:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:46:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:46:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:46:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:46:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:46:21 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:46:21 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:46:22 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:46:23 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:46:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b83e8a6ea044be2a9e3c87c5fdc047ce9a52d1a64e48f8330d9a19002ecffe1`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 300.1 KB (300117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9949bdfbb1d296dd158f8c2bb959f96c8da162a0d579f68fa3f5a4af58bed5b`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c5cc316af29a89f9a1d4e279b5d1bb964095a15795647d013f40921bc808c3`  
		Last Modified: Wed, 14 Apr 2021 19:47:54 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6670cc680ce5e5d9a0adfc380fe4a89ac2a2dcef5a7adeb874967a356e6742`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1a41623f53d582c8b503ae859f6ae98c7c0695eddb11bdbf8514b9b914955c3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13639723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4b837694902a1a259a4915444feda59d895ed37ffbef66b8518b9a884f029c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:39:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 19:39:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 19:39:34 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:39:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:39:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:39:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:39:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:39:43 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:39:45 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:39:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:39:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:39:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:39:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:39:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:39:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:39:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:39:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:39:56 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:39:57 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:39:58 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:39:59 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:40:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b239ad5e698454501b0de011bffea35a660806a0b85a6141776581e3a98bc467`  
		Last Modified: Wed, 14 Apr 2021 19:41:24 GMT  
		Size: 299.2 KB (299210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0460b038be93717158ad9cdb6f83768b7129eaf4fcaef8620adc7509d0e5fe`  
		Last Modified: Wed, 14 Apr 2021 19:41:23 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0905d1ca8c4f74966ae8a7b5ebe8fdb33854c4a759d543d767dd9a0add81f155`  
		Last Modified: Wed, 14 Apr 2021 19:41:29 GMT  
		Size: 10.9 MB (10925348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f02da274f552e184a7fa5527990e666d77c70e3715a0d96b7588e7433b3022a`  
		Last Modified: Wed, 14 Apr 2021 19:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:789a609d1ac52d0bed8718bab07beff0633df8333c8f88a4a54ccc6fa14bfb1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13616003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86fab65bcfd86f1922cd2ec38aa336d5c219f99ed0d0878dede9732c770b2113`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:59:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 18:59:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 18:59:56 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:00:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:00:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:00:06 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:00:07 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:00:08 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:00:09 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:00:10 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:00:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:00:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:00:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:00:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:00:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:00:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:00:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:00:22 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:00:23 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:00:25 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:00:26 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:00:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96638d6a34d0588d1723cae433a6176b83e4bec10cb3a37ffac1891313dd144`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 300.4 KB (300352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27e448c61e8710f135f93f0f19db0e1e20005299e4e28dfcbba2fc048075b11`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955bb49759c02742bb3fe501b864201c3b2a349f8253b73d7114ba39a816ac02`  
		Last Modified: Wed, 14 Apr 2021 19:01:54 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f923159f69301bb290369ef4804ec8ef52d3d159d531976474f8d34d3dc54`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:f551e1db7910e2d5235d303760aff5b514fc6e8b49d8d67d434bb23c40ac25db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13356454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982bd235f46e537404cdab42c3dfb3d0058f97ed5d7984f2e71ad8734adcc6a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:09:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 22:09:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 22:09:24 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 22:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 22:09:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:09:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 22:10:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 22:10:06 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 22:10:15 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 22:10:22 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 22:10:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 22:10:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 22:10:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 22:10:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 22:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 22:11:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 22:11:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 22:11:14 GMT
EXPOSE 80
# Wed, 14 Apr 2021 22:11:20 GMT
EXPOSE 443
# Wed, 14 Apr 2021 22:11:27 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 22:11:35 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 22:11:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93dd31358a6e859a05bb506b946720f02c7ec7969776d811b20eaaa84508cd7`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 302.3 KB (302339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8077b8c9cca163d9a34281a866cf5fe991ff8c160ebd1ab1b617c6b722ec690`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55884816b8eca8150db9473989410e372c69c5431deb51a6cacd029895cf3dd6`  
		Last Modified: Wed, 14 Apr 2021 22:15:43 GMT  
		Size: 10.2 MB (10241380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51efee06e0a650ff5f146fc54a695d4bf2b44e19da18120fdc494982d52cdd62`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - linux; s390x

```console
$ docker pull caddy@sha256:68aaf625a22bff4e71edf895129baa2d562765c24ac81a5c68aff2995ebf89c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14146947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfd454f0dfa64ee1a952f9ed74a3f3bda3688a9565f062c3ea37e48b54eb210`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:07:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:07:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:07:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:07:26 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:07:27 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:07:27 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:07:30 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:07:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab58470b754d248933aa56b48394e3ee4db4561d430d23ea378f0371ca59cb`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd514b608428ea44dae7dc67e641a276593e7715178d86d7702153521de849d7`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a437814dab55b178c71f55598a70d0b532b3f645bdeb43e89244a6ebcde01446`  
		Last Modified: Wed, 14 Apr 2021 20:08:18 GMT  
		Size: 11.3 MB (11272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be9af105c69ee35fec76e8c0dbde8c8ba61c774b7d354e9c9fc8f538e8155`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-alpine`

```console
$ docker pull caddy@sha256:fa1ae85dc9b12ee47e98d7ef21db409eada3ed48f1865e4b1f1dd78f417132fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6fbf52298c46c55c572670b5395ecaee5d399338003c9bb4e4abed875c542f4f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.7 MB (14728953 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7395cc3713b2ca5574a9b4aafc468a1533d16582efe47dcab74ed547540d698a`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:10:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:10:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:10:49 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:10:52 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:10:53 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:10:53 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:10:53 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:10:54 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:10:54 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:10:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:10:55 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:10:56 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:10:56 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:10:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a0cd9cca5be9b30bbc70611052d1456502e1f338ce4b14946233b21cd6a9a`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 300.0 KB (300016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5666523658a43fbbdff6b8fca498a988f4dcecc3ce027f1701414658c21d4ea`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b097228407f13a161f68b188b0a4f255855b64d84e7b076745a744d5aa7ed8cf`  
		Last Modified: Wed, 14 Apr 2021 20:11:49 GMT  
		Size: 11.6 MB (11622383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40682d93cc09b4592a1b9c08d48d0a956b5eef4f123d80d1a12942482edb6aab`  
		Last Modified: Wed, 14 Apr 2021 20:11:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:0df9df9725cab39fe073887c98b54bf7bf1c96b3ed0e23916737c7c4877576c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13856181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fce1c33ce4509195edc1c67d2dcd15c6c5fc0b35cec2e90714ec3007739600eb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:45:19 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 19:45:33 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 19:45:36 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:45:54 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:46:03 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:46:04 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:46:05 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:46:07 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:46:08 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:46:10 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:46:11 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:46:13 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:46:16 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:46:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:46:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:46:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:46:20 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:46:21 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:46:21 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:46:22 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:46:23 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:46:24 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b83e8a6ea044be2a9e3c87c5fdc047ce9a52d1a64e48f8330d9a19002ecffe1`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 300.1 KB (300117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9949bdfbb1d296dd158f8c2bb959f96c8da162a0d579f68fa3f5a4af58bed5b`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c5cc316af29a89f9a1d4e279b5d1bb964095a15795647d013f40921bc808c3`  
		Last Modified: Wed, 14 Apr 2021 19:47:54 GMT  
		Size: 10.9 MB (10944831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6670cc680ce5e5d9a0adfc380fe4a89ac2a2dcef5a7adeb874967a356e6742`  
		Last Modified: Wed, 14 Apr 2021 19:47:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:1a41623f53d582c8b503ae859f6ae98c7c0695eddb11bdbf8514b9b914955c3d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13639723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4b837694902a1a259a4915444feda59d895ed37ffbef66b8518b9a884f029c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:39:25 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 19:39:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 19:39:34 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:39:38 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:39:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:39:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:39:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:39:43 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:39:45 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:39:46 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:39:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:39:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:39:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:39:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:39:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:39:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:39:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:39:56 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:39:57 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:39:58 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:39:59 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:40:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b239ad5e698454501b0de011bffea35a660806a0b85a6141776581e3a98bc467`  
		Last Modified: Wed, 14 Apr 2021 19:41:24 GMT  
		Size: 299.2 KB (299210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0460b038be93717158ad9cdb6f83768b7129eaf4fcaef8620adc7509d0e5fe`  
		Last Modified: Wed, 14 Apr 2021 19:41:23 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0905d1ca8c4f74966ae8a7b5ebe8fdb33854c4a759d543d767dd9a0add81f155`  
		Last Modified: Wed, 14 Apr 2021 19:41:29 GMT  
		Size: 10.9 MB (10925348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f02da274f552e184a7fa5527990e666d77c70e3715a0d96b7588e7433b3022a`  
		Last Modified: Wed, 14 Apr 2021 19:41:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:789a609d1ac52d0bed8718bab07beff0633df8333c8f88a4a54ccc6fa14bfb1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13616003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86fab65bcfd86f1922cd2ec38aa336d5c219f99ed0d0878dede9732c770b2113`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 18:59:52 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 18:59:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 18:59:56 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 19:00:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 19:00:05 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 19:00:06 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 19:00:07 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 19:00:08 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 19:00:09 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 19:00:10 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 19:00:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 19:00:14 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 19:00:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 19:00:16 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 19:00:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 19:00:20 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 19:00:21 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 19:00:22 GMT
EXPOSE 80
# Wed, 14 Apr 2021 19:00:23 GMT
EXPOSE 443
# Wed, 14 Apr 2021 19:00:25 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 19:00:26 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 19:00:28 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96638d6a34d0588d1723cae433a6176b83e4bec10cb3a37ffac1891313dd144`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 300.4 KB (300352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27e448c61e8710f135f93f0f19db0e1e20005299e4e28dfcbba2fc048075b11`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955bb49759c02742bb3fe501b864201c3b2a349f8253b73d7114ba39a816ac02`  
		Last Modified: Wed, 14 Apr 2021 19:01:54 GMT  
		Size: 10.6 MB (10598977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639f923159f69301bb290369ef4804ec8ef52d3d159d531976474f8d34d3dc54`  
		Last Modified: Wed, 14 Apr 2021 19:01:50 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:f551e1db7910e2d5235d303760aff5b514fc6e8b49d8d67d434bb23c40ac25db
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13356454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982bd235f46e537404cdab42c3dfb3d0058f97ed5d7984f2e71ad8734adcc6a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:09:04 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 22:09:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 22:09:24 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 22:09:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 22:09:51 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:09:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 22:10:01 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 22:10:06 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 22:10:15 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 22:10:22 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 22:10:32 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 22:10:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 22:10:46 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 22:10:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 22:10:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 22:11:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 22:11:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 22:11:14 GMT
EXPOSE 80
# Wed, 14 Apr 2021 22:11:20 GMT
EXPOSE 443
# Wed, 14 Apr 2021 22:11:27 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 22:11:35 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 22:11:41 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d93dd31358a6e859a05bb506b946720f02c7ec7969776d811b20eaaa84508cd7`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 302.3 KB (302339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8077b8c9cca163d9a34281a866cf5fe991ff8c160ebd1ab1b617c6b722ec690`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55884816b8eca8150db9473989410e372c69c5431deb51a6cacd029895cf3dd6`  
		Last Modified: Wed, 14 Apr 2021 22:15:43 GMT  
		Size: 10.2 MB (10241380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51efee06e0a650ff5f146fc54a695d4bf2b44e19da18120fdc494982d52cdd62`  
		Last Modified: Wed, 14 Apr 2021 22:15:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:68aaf625a22bff4e71edf895129baa2d562765c24ac81a5c68aff2995ebf89c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.1 MB (14146947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfd454f0dfa64ee1a952f9ed74a3f3bda3688a9565f062c3ea37e48b54eb210`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 14 Apr 2021 20:07:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"
# Wed, 14 Apr 2021 20:07:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 14 Apr 2021 20:07:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='7112a03bf341a4ccc5332b5ea715de9a68316d2aa2f468bdc263b192448ce412e002acfda68bd0606088b35c5de1f2e93f2aa64ccc065a039f87ee34e0b85b98' ;; 		armhf)   binArch='armv6'; checksum='a597dbfbd277648881cf51739382a509e5014b3342c78e444f6a680f93836d46c12fc1294e200358fd4a0a40688c5582c81bff14dffd0bba5303170a4d274014' ;; 		armv7)   binArch='armv7'; checksum='99e7703ffa9dd8f636f4624c0972fd3d4af01523953ebf487b919ce93e1989b5513785dd9e902326423eb334bb22dddbcccab382f46763ec11c43c9e513f7c38' ;; 		aarch64) binArch='arm64'; checksum='ef1e44293a935b05602524dbab96b51c862864b8a36c7de48b3329dab9b8a4b7d1930460868fded3afb3a74bdfb5a1c1c0ba46f1401edf648a370c0f7be8a05b' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='62e4a191cae8a1a023ab2653b76439cd4182ca49af4f00bff56507f9f1f4af3e72716a59c59ff157efa87c655110fb2491125baae72590719870dc795d19538d' ;; 		s390x)   binArch='s390x'; checksum='48cac248c29218e153d76408b172510f4f02e3fe7f7b2209371d2c69ed46d2bfa1f572f46390a00eda6f9296a8cac744a36e21cae6df791bd9d98f22b43ea42b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 14 Apr 2021 20:07:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:07:26 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 14 Apr 2021 20:07:27 GMT
ENV XDG_DATA_HOME=/data
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/config]
# Wed, 14 Apr 2021 20:07:27 GMT
VOLUME [/data]
# Wed, 14 Apr 2021 20:07:27 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 14 Apr 2021 20:07:28 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 14 Apr 2021 20:07:29 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 80
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 443
# Wed, 14 Apr 2021 20:07:29 GMT
EXPOSE 2019
# Wed, 14 Apr 2021 20:07:30 GMT
WORKDIR /srv
# Wed, 14 Apr 2021 20:07:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dab58470b754d248933aa56b48394e3ee4db4561d430d23ea378f0371ca59cb`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 300.5 KB (300471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd514b608428ea44dae7dc67e641a276593e7715178d86d7702153521de849d7`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 5.8 KB (5832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a437814dab55b178c71f55598a70d0b532b3f645bdeb43e89244a6ebcde01446`  
		Last Modified: Wed, 14 Apr 2021 20:08:18 GMT  
		Size: 11.3 MB (11272061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412be9af105c69ee35fec76e8c0dbde8c8ba61c774b7d354e9c9fc8f538e8155`  
		Last Modified: Wed, 14 Apr 2021 20:08:16 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder`

```console
$ docker pull caddy@sha256:8d8978b2b2ca750e8ad69be7fbdf2f87903201cb5adb02b6e67aa5744f70d3b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:6740d877ef515ceac8a37a496899fea4d7607bd9831a4a6c990949964ccf3536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119554161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48e0382f0f224a95381e7fdb346fe40e28931bdec03923e00db3699d75eec90`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:29:08 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:29:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:29:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:25:19 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:27:21 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:27:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:27:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:27:22 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 01:56:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 01:56:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 01:56:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 01:56:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 01:56:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22b54d2d4342f88201f48db57cae1f7edbacae870ee13d7962f999edd7529a9`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5898d3d0f1f95fd666f764bf918c1656be6169868335cb63bc428a5ef47cf32`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7bf786162598b899ee14cad74bdc1c8a634091a242e88aecef7426389cc2c4`  
		Last Modified: Thu, 06 May 2021 23:32:32 GMT  
		Size: 106.8 MB (106834379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6e1c1f19605c012184b2d0a8839483fcd208ac6cec2f7960703fdd1175dfcf`  
		Last Modified: Thu, 06 May 2021 23:32:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8271517dcb3cc152671658ffe8a14ad9d506a93ecdf782757e9ae05c710b62b5`  
		Last Modified: Fri, 07 May 2021 01:56:41 GMT  
		Size: 8.3 MB (8326465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9f2fd9dcaaae8f453297e27e74f09fe28520c7c7c8665bc59870f9fabee0f7`  
		Last Modified: Fri, 07 May 2021 01:56:40 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523069c0450345d7a7e25d5d975f68003c2311e50b473eaa1ea30f0586fdc2a`  
		Last Modified: Fri, 07 May 2021 01:56:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:980832939db15c6c49b8766e2280086f9f77df42313ceaa4b704ca9f312de749
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114743259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3834a17da42d3f0311833167382a844bb02d9fe3054be01d4fc62f70649d8b6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:19:47 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:19:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:19:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:34:21 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 21:37:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:37:16 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:37:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:37:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:37:22 GMT
WORKDIR /go
# Thu, 06 May 2021 22:09:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:09:58 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 06 May 2021 22:09:59 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 06 May 2021 22:10:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 May 2021 22:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 May 2021 22:10:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 May 2021 22:10:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c231c184d802a569805e44837dd1ea2cb0522bb03ca5763ef5ed9fae5896c`  
		Last Modified: Wed, 14 Apr 2021 21:15:05 GMT  
		Size: 281.0 KB (280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ca9e585b85be2e7ddaaf213e22bdb986eba4da2a8cc4d8b45f762752e17df`  
		Last Modified: Wed, 14 Apr 2021 21:15:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207e70e1aafbd96d35878b34eac9d70629c7d0d5c95d6a6d595497dc16384314`  
		Last Modified: Thu, 06 May 2021 21:40:38 GMT  
		Size: 102.7 MB (102690906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafdae0ee7bc20a8ce52360fd0237c2d561f4dda69b5221756ee2fb08f3a25e9`  
		Last Modified: Thu, 06 May 2021 21:40:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37943907ed09326e414a914b2f13d600e2a94f806a260c7941e9930dc8e914db`  
		Last Modified: Thu, 06 May 2021 22:10:53 GMT  
		Size: 7.9 MB (7943728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a400fa97dfdb53333f7d2d7405ff6f39461b2e43eb8337b0b06fff17c362074c`  
		Last Modified: Thu, 06 May 2021 22:10:52 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fed79ee3fc09876eea261ab1cde8d9107b041a4d873ab2dbcacdc0f0b0db47`  
		Last Modified: Thu, 06 May 2021 22:10:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6a27d36624d8ceafd50f9caf199d8583315839b6e47617242194192b6443fad3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113547980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13dd897b9d3a097309d0364885377e102cd91c4dcec23ffd64375520f0029b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:28:16 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:28:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:28:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:22:53 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:25:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:25:38 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:25:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:25:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:25:46 GMT
WORKDIR /go
# Fri, 07 May 2021 02:33:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:33:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 02:33:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 02:33:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 02:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 02:33:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 02:34:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a884c3a8500725e0f08f924091ec61ae3e3acee3b0ffe5839b06f874ee63dc08`  
		Last Modified: Wed, 14 Apr 2021 22:45:08 GMT  
		Size: 280.1 KB (280078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f87f08a98de1e7cb636267b626d4e644775ff7962ea1ff9b4813f740b89e67`  
		Last Modified: Wed, 14 Apr 2021 22:45:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73018330efc261efdcdccd072ee7b6ea3dc05bab6b4760a1ec828924d12acf96`  
		Last Modified: Thu, 06 May 2021 23:31:44 GMT  
		Size: 102.5 MB (102483682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12ff58945623ccdd317243b312562a87a60534d35bb0a88f1e2bdd4b800450a`  
		Last Modified: Thu, 06 May 2021 23:31:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada1f2ae57155d23410debd2de0fed3f494ac4cedb2d716f10ac64aa8f49350c`  
		Last Modified: Fri, 07 May 2021 02:34:45 GMT  
		Size: 7.2 MB (7154830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132f297784ed0d2a64f3581da395b458a6ad21b2a884c3dbabf79410415362c`  
		Last Modified: Fri, 07 May 2021 02:34:44 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd68f4d45c90ed4b3be4d5335c923e68cdd3317597b2575fabbdacf45f38fc`  
		Last Modified: Fri, 07 May 2021 02:34:44 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b7a5c24ebc428a66842618e2ad381544cd986e997f453e0d9a2f671ad0bfa2f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114864048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d2bfdb86bdd828c562eee0c551e06aa4e79276d99135f5bd2b7cfe798aed31`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:09 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:46:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:46:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:39:55 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 22:41:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:41:48 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:41:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:41:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:41:52 GMT
WORKDIR /go
# Fri, 07 May 2021 01:16:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:16:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 01:16:57 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 01:16:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 01:17:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 01:17:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 01:17:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2150ab4b89a5dc832780f442998074db1582348dca0eb60d6b79b59df025f25f`  
		Last Modified: Wed, 14 Apr 2021 21:00:21 GMT  
		Size: 281.2 KB (281220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9d22c0ca7447b1a1b25889675e84f2ed68ecd519fdc513796712138820633b`  
		Last Modified: Wed, 14 Apr 2021 21:00:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328eb5d68387c28c06740854a27e1f61291595913519fa3169b91f9b46bb9ca`  
		Last Modified: Thu, 06 May 2021 22:47:05 GMT  
		Size: 102.2 MB (102151470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2893b907041eb1a7fdd24da73ae2cfa10e6f9286ae37b7d7b77b3b322d2fafe1`  
		Last Modified: Thu, 06 May 2021 22:46:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c9359228d2ef91a5f155bf4eb9cacf4d7a44958e4374cc497939e854cbedc`  
		Last Modified: Fri, 07 May 2021 01:17:51 GMT  
		Size: 8.5 MB (8518410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b89f42f011d15cd85b0d0d03916e5eaa1015e732785e1508631c9d52a7ac3`  
		Last Modified: Fri, 07 May 2021 01:17:49 GMT  
		Size: 1.2 MB (1201538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f53e0aeae2a617ee063849011cb33db824b4ba6b3970945825fa7aed9143db`  
		Last Modified: Fri, 07 May 2021 01:17:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:91017bdca5b5a6e529ba9dbbf8b4cc0f1abad484dd2a19ff8162e5a20f1b7470
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114013692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c636d928211d0eebf80ad41447aae081460c4d3673fbb846379e0f71a65c581c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:05 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:57:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:35:58 GMT
ENV GOLANG_VERSION=1.15.12
# Fri, 07 May 2021 00:38:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:38:24 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:38:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:38:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:38:53 GMT
WORKDIR /go
# Fri, 07 May 2021 08:18:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:18:28 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 08:18:33 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 08:18:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 08:19:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 08:19:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 08:19:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dca7bf08f7e7ef8f1c651b5ba53ba748e66f5a75400b38f67596867bfae4e2`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 283.2 KB (283201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d495ca184c89fdc74ec1ec1cc670ff41be844b29174141c4602ac1400b0645`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d75cc8304f9250be10afcbb80447f234d1f01911e86274118bb6fdc34ed48`  
		Last Modified: Fri, 07 May 2021 00:44:07 GMT  
		Size: 100.8 MB (100812628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0997c196aa13c6e561f3432b7239d95ee90562c507e5a8c4f21acfcf1e17f5e3`  
		Last Modified: Fri, 07 May 2021 00:43:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6e06aa8363e1138fed17e9f2a879be30ac49ebdee6931f49ea76200a4cab3`  
		Last Modified: Fri, 07 May 2021 08:22:00 GMT  
		Size: 8.9 MB (8939878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedccec34d2dc5617dde35e772984f1c60c1cf730c13faeef29d2ecf217b24df`  
		Last Modified: Fri, 07 May 2021 08:21:58 GMT  
		Size: 1.2 MB (1170522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b959e44e74065aea1788a48f30813a54b7121ff398a293ed94b2d6d370f57d8`  
		Last Modified: Fri, 07 May 2021 08:21:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0de068b7cd9c14fc067305805ff915769769fc9cd7d7daafe247873960c9e481
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118429363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d6106b96bf5579d67b5457592a4408517a6015fbcd4144b7e04407d47a04d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:47:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:47:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:29:16 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:32:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:32:38 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:32:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:32:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:32:41 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 02:02:16 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 02:02:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 02:02:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 02:02:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 02:02:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c45d0e43ef7a36e47dfc16916a076f7ba26b656842380c26207ad30f5c8b`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 281.3 KB (281343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1645d6cbfccd2924337f37dc819e7edc27989ead8bc679441954a0e483c24`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e82967ca9bc6ee6bdd75fdc4f9b9000c6fcb2c25b0d754591f4ea080d22c48`  
		Last Modified: Thu, 06 May 2021 23:36:04 GMT  
		Size: 105.9 MB (105944163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f7138aca5efa6f3f896323bc1d8d7e86ac97dc43934f657be7b59764fd1a93`  
		Last Modified: Thu, 06 May 2021 23:35:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fc295bef09a7a41613606b2fab0bb9a2f237a924f638bbc1471e4cf7e8b91`  
		Last Modified: Fri, 07 May 2021 02:03:09 GMT  
		Size: 8.4 MB (8370195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e637a1eb5e336e7d0f477e2470ceb6a4501f134379834cd84e644993a10c733c`  
		Last Modified: Fri, 07 May 2021 02:03:08 GMT  
		Size: 1.3 MB (1264520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eeaadfe4374cccb5c1a67a72e18041ebe4ad77c344002126dc56db880377cfa`  
		Last Modified: Fri, 07 May 2021 02:03:08 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:7c26382633835010d4cfd02b1c6fa418ce94cd4165e8eb946128fe754fc224c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2640840527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7d48302374c8837dcb0b4a7eafbf5ab92ad9e14c7961978e4d6411547ce085`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:40:41 GMT
ENV GOLANG_VERSION=1.15.12
# Wed, 12 May 2021 12:43:35 GMT
RUN $url = 'https://dl.google.com/go/go1.15.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '313e5ebc59b497319c4c3f9560322fcc20f7bc3b4e47494afc3b2d63a42fb2a5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:43:38 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 19:53:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:53:05 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 19:53:06 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:53:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 19:53:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 19:53:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e10fb8a78b4fccaf2e1f27fade2351acbab7977f469077dbe3d61137a83bd1b`  
		Last Modified: Wed, 12 May 2021 12:59:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611233319702edb459b2c018bda3a84c557bdaed90507b5265b2802d845363c0`  
		Last Modified: Wed, 12 May 2021 12:59:39 GMT  
		Size: 134.1 MB (134130080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bae92e561d0c550e6481307d686ba1fd33b1c5ac6ea31411fb23e6db83b80df`  
		Last Modified: Wed, 12 May 2021 12:59:07 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206ea1b195825780737f5b6198def0bcdad5960c0341b1151836d1c07b9d2162`  
		Last Modified: Wed, 12 May 2021 20:05:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c2b185bf4960bb532474f7c1c09eed87a687f35127349952d45f9fbed859a1`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a954bd53bbccc7e000e23a03005396cf73110a1eef4cbb2b5713b094303abb`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b33214b7398e925aad6bb865e8c77d126584dec2ee7f66108665c4b2d407a57`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a997270f53d496525fd665c09144ce7851254655d8651fdbb6f0d8b879a7c67e`  
		Last Modified: Wed, 12 May 2021 20:05:37 GMT  
		Size: 1.7 MB (1700479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57110530a8b452cb9ec0c7a6cefccc83019117e7d5477cb24669f1cde954240`  
		Last Modified: Wed, 12 May 2021 20:05:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:906461df38b01faa5b735a5c09cb4cebeed6d8edb2556dc81cc9dc80923146e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5983275276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51d50a0e24be6c3ffc1c47427c3ce640d5e24f0e908ee635159d34278f463e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:43:55 GMT
ENV GOLANG_VERSION=1.15.12
# Wed, 12 May 2021 12:48:02 GMT
RUN $url = 'https://dl.google.com/go/go1.15.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '313e5ebc59b497319c4c3f9560322fcc20f7bc3b4e47494afc3b2d63a42fb2a5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:48:04 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 19:53:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:53:43 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 19:53:44 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:53:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 19:55:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 19:55:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e10c98a45913a3ce79e3502f8ad0b4a47ee36123faf47dcbf2795b50878648`  
		Last Modified: Wed, 12 May 2021 12:59:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b9313f31970ae7f9cdeff1169da12a64965a580063923bf01a3f81af1b8c4`  
		Last Modified: Wed, 12 May 2021 13:02:38 GMT  
		Size: 144.0 MB (143977383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b7390fa519672498ab6ced5bce95384a4922d59dbb35dd0725b1a6dedf33dd`  
		Last Modified: Wed, 12 May 2021 12:59:51 GMT  
		Size: 1.6 KB (1581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0a2adda3b5f16542c4a28642492806dd2009f6bc3032c3b9ef873715138d99`  
		Last Modified: Wed, 12 May 2021 20:05:51 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b9a511fdc0e9ddf64e9049876b9797f277670c797fa8839f5c4f623dc3558e`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90ade527b07762be1cffc2b787cc902d0f5836e4d75d3b745ecc24491769bab`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c752fd61bb0787576c60601f38f5ded35e90a6f86a39e72606bddeb9fb3603`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706f2f07a14a0961a5455784d51275ceaa6ad9ed410035c4b552ec7296fd0268`  
		Last Modified: Wed, 12 May 2021 20:05:58 GMT  
		Size: 7.0 MB (7042421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ae4915980d2bfd94575229474b5b9021fb64dc7781d5a14a075db51743e35c`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-alpine`

```console
$ docker pull caddy@sha256:e06d5cdcee711e9580fe595e8f03d31e17394fba29865720a64ddee23892b4a7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.3.0-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6740d877ef515ceac8a37a496899fea4d7607bd9831a4a6c990949964ccf3536
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.6 MB (119554161 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c48e0382f0f224a95381e7fdb346fe40e28931bdec03923e00db3699d75eec90`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:29:08 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:29:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:29:09 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:25:19 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:27:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:27:21 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:27:21 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:27:22 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:27:22 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:04 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:04 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 01:56:04 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 01:56:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 01:56:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 01:56:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 01:56:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22b54d2d4342f88201f48db57cae1f7edbacae870ee13d7962f999edd7529a9`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 280.9 KB (280879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5898d3d0f1f95fd666f764bf918c1656be6169868335cb63bc428a5ef47cf32`  
		Last Modified: Wed, 14 Apr 2021 21:35:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7bf786162598b899ee14cad74bdc1c8a634091a242e88aecef7426389cc2c4`  
		Last Modified: Thu, 06 May 2021 23:32:32 GMT  
		Size: 106.8 MB (106834379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6e1c1f19605c012184b2d0a8839483fcd208ac6cec2f7960703fdd1175dfcf`  
		Last Modified: Thu, 06 May 2021 23:32:16 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8271517dcb3cc152671658ffe8a14ad9d506a93ecdf782757e9ae05c710b62b5`  
		Last Modified: Fri, 07 May 2021 01:56:41 GMT  
		Size: 8.3 MB (8326465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf9f2fd9dcaaae8f453297e27e74f09fe28520c7c7c8665bc59870f9fabee0f7`  
		Last Modified: Fri, 07 May 2021 01:56:40 GMT  
		Size: 1.3 MB (1311156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523069c0450345d7a7e25d5d975f68003c2311e50b473eaa1ea30f0586fdc2a`  
		Last Modified: Fri, 07 May 2021 01:56:40 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:980832939db15c6c49b8766e2280086f9f77df42313ceaa4b704ca9f312de749
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114743259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3834a17da42d3f0311833167382a844bb02d9fe3054be01d4fc62f70649d8b6`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:49 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Wed, 14 Apr 2021 18:49:50 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:19:47 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:19:50 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:19:52 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:34:21 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 21:37:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:37:16 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:37:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:37:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:37:22 GMT
WORKDIR /go
# Thu, 06 May 2021 22:09:57 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:09:58 GMT
ENV XCADDY_VERSION=v0.1.9
# Thu, 06 May 2021 22:09:59 GMT
ENV CADDY_VERSION=v2.3.0
# Thu, 06 May 2021 22:10:00 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 06 May 2021 22:10:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 06 May 2021 22:10:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 06 May 2021 22:10:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76c231c184d802a569805e44837dd1ea2cb0522bb03ca5763ef5ed9fae5896c`  
		Last Modified: Wed, 14 Apr 2021 21:15:05 GMT  
		Size: 281.0 KB (280982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8ca9e585b85be2e7ddaaf213e22bdb986eba4da2a8cc4d8b45f762752e17df`  
		Last Modified: Wed, 14 Apr 2021 21:15:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:207e70e1aafbd96d35878b34eac9d70629c7d0d5c95d6a6d595497dc16384314`  
		Last Modified: Thu, 06 May 2021 21:40:38 GMT  
		Size: 102.7 MB (102690906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafdae0ee7bc20a8ce52360fd0237c2d561f4dda69b5221756ee2fb08f3a25e9`  
		Last Modified: Thu, 06 May 2021 21:40:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37943907ed09326e414a914b2f13d600e2a94f806a260c7941e9930dc8e914db`  
		Last Modified: Thu, 06 May 2021 22:10:53 GMT  
		Size: 7.9 MB (7943728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a400fa97dfdb53333f7d2d7405ff6f39461b2e43eb8337b0b06fff17c362074c`  
		Last Modified: Thu, 06 May 2021 22:10:52 GMT  
		Size: 1.2 MB (1221675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fed79ee3fc09876eea261ab1cde8d9107b041a4d873ab2dbcacdc0f0b0db47`  
		Last Modified: Thu, 06 May 2021 22:10:51 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:6a27d36624d8ceafd50f9caf199d8583315839b6e47617242194192b6443fad3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.5 MB (113547980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bc13dd897b9d3a097309d0364885377e102cd91c4dcec23ffd64375520f0029b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:50 GMT
ADD file:d844cc7b5e00fb62be39d903a2fb4a08f700e75112c8eef1f31101e846ed010d in / 
# Wed, 14 Apr 2021 18:57:52 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:28:16 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:28:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:28:26 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:22:53 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:25:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:25:38 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:25:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:25:44 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:25:46 GMT
WORKDIR /go
# Fri, 07 May 2021 02:33:54 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:33:55 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 02:33:56 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 02:33:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 02:33:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 02:33:59 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 02:34:00 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:420c7481a3a76d5d12df768d2745ddbe40357df0af780c756a5a7d1f2a43d288`  
		Last Modified: Wed, 14 Apr 2021 18:58:46 GMT  
		Size: 2.4 MB (2409178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a884c3a8500725e0f08f924091ec61ae3e3acee3b0ffe5839b06f874ee63dc08`  
		Last Modified: Wed, 14 Apr 2021 22:45:08 GMT  
		Size: 280.1 KB (280078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f87f08a98de1e7cb636267b626d4e644775ff7962ea1ff9b4813f740b89e67`  
		Last Modified: Wed, 14 Apr 2021 22:45:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73018330efc261efdcdccd072ee7b6ea3dc05bab6b4760a1ec828924d12acf96`  
		Last Modified: Thu, 06 May 2021 23:31:44 GMT  
		Size: 102.5 MB (102483682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12ff58945623ccdd317243b312562a87a60534d35bb0a88f1e2bdd4b800450a`  
		Last Modified: Thu, 06 May 2021 23:31:14 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada1f2ae57155d23410debd2de0fed3f494ac4cedb2d716f10ac64aa8f49350c`  
		Last Modified: Fri, 07 May 2021 02:34:45 GMT  
		Size: 7.2 MB (7154830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6132f297784ed0d2a64f3581da395b458a6ad21b2a884c3dbabf79410415362c`  
		Last Modified: Fri, 07 May 2021 02:34:44 GMT  
		Size: 1.2 MB (1219497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd68f4d45c90ed4b3be4d5335c923e68cdd3317597b2575fabbdacf45f38fc`  
		Last Modified: Fri, 07 May 2021 02:34:44 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:b7a5c24ebc428a66842618e2ad381544cd986e997f453e0d9a2f671ad0bfa2f4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.9 MB (114864048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7d2bfdb86bdd828c562eee0c551e06aa4e79276d99135f5bd2b7cfe798aed31`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:54 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Wed, 14 Apr 2021 18:42:55 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:09 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:46:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:46:37 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:39:55 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 22:41:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:41:48 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:41:49 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:41:51 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:41:52 GMT
WORKDIR /go
# Fri, 07 May 2021 01:16:56 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:16:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 01:16:57 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 01:16:58 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 01:17:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 01:17:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 01:17:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2150ab4b89a5dc832780f442998074db1582348dca0eb60d6b79b59df025f25f`  
		Last Modified: Wed, 14 Apr 2021 21:00:21 GMT  
		Size: 281.2 KB (281220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a9d22c0ca7447b1a1b25889675e84f2ed68ecd519fdc513796712138820633b`  
		Last Modified: Wed, 14 Apr 2021 21:00:23 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2328eb5d68387c28c06740854a27e1f61291595913519fa3169b91f9b46bb9ca`  
		Last Modified: Thu, 06 May 2021 22:47:05 GMT  
		Size: 102.2 MB (102151470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2893b907041eb1a7fdd24da73ae2cfa10e6f9286ae37b7d7b77b3b322d2fafe1`  
		Last Modified: Thu, 06 May 2021 22:46:39 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a02c9359228d2ef91a5f155bf4eb9cacf4d7a44958e4374cc497939e854cbedc`  
		Last Modified: Fri, 07 May 2021 01:17:51 GMT  
		Size: 8.5 MB (8518410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea7b89f42f011d15cd85b0d0d03916e5eaa1015e732785e1508631c9d52a7ac3`  
		Last Modified: Fri, 07 May 2021 01:17:49 GMT  
		Size: 1.2 MB (1201538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3f53e0aeae2a617ee063849011cb33db824b4ba6b3970945825fa7aed9143db`  
		Last Modified: Fri, 07 May 2021 01:17:49 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:91017bdca5b5a6e529ba9dbbf8b4cc0f1abad484dd2a19ff8162e5a20f1b7470
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.0 MB (114013692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c636d928211d0eebf80ad41447aae081460c4d3673fbb846379e0f71a65c581c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:57:05 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:57:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:57:16 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:35:58 GMT
ENV GOLANG_VERSION=1.15.12
# Fri, 07 May 2021 00:38:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:38:24 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:38:32 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:38:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:38:53 GMT
WORKDIR /go
# Fri, 07 May 2021 08:18:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:18:28 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 08:18:33 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 08:18:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 08:19:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 08:19:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 08:19:12 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dca7bf08f7e7ef8f1c651b5ba53ba748e66f5a75400b38f67596867bfae4e2`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 283.2 KB (283201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d495ca184c89fdc74ec1ec1cc670ff41be844b29174141c4602ac1400b0645`  
		Last Modified: Wed, 14 Apr 2021 23:06:16 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6d75cc8304f9250be10afcbb80447f234d1f01911e86274118bb6fdc34ed48`  
		Last Modified: Fri, 07 May 2021 00:44:07 GMT  
		Size: 100.8 MB (100812628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0997c196aa13c6e561f3432b7239d95ee90562c507e5a8c4f21acfcf1e17f5e3`  
		Last Modified: Fri, 07 May 2021 00:43:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb6e06aa8363e1138fed17e9f2a879be30ac49ebdee6931f49ea76200a4cab3`  
		Last Modified: Fri, 07 May 2021 08:22:00 GMT  
		Size: 8.9 MB (8939878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedccec34d2dc5617dde35e772984f1c60c1cf730c13faeef29d2ecf217b24df`  
		Last Modified: Fri, 07 May 2021 08:21:58 GMT  
		Size: 1.2 MB (1170522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b959e44e74065aea1788a48f30813a54b7121ff398a293ed94b2d6d370f57d8`  
		Last Modified: Fri, 07 May 2021 08:21:58 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0de068b7cd9c14fc067305805ff915769769fc9cd7d7daafe247873960c9e481
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.4 MB (118429363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86d6106b96bf5579d67b5457592a4408517a6015fbcd4144b7e04407d47a04d3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:46:59 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:47:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:47:00 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:29:16 GMT
ENV GOLANG_VERSION=1.15.12
# Thu, 06 May 2021 23:32:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='387' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.15.12.src.tar.gz'; 	sha256='1c6911937df4a277fa74e7b7efc3d08594498c4c4adc0b6c4ae3566137528091'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:32:38 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:32:38 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:32:40 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:32:41 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:15 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:15 GMT
ENV XCADDY_VERSION=v0.1.9
# Fri, 07 May 2021 02:02:16 GMT
ENV CADDY_VERSION=v2.3.0
# Fri, 07 May 2021 02:02:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Fri, 07 May 2021 02:02:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Fri, 07 May 2021 02:02:20 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Fri, 07 May 2021 02:02:21 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c29c45d0e43ef7a36e47dfc16916a076f7ba26b656842380c26207ad30f5c8b`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 281.3 KB (281343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f1645d6cbfccd2924337f37dc819e7edc27989ead8bc679441954a0e483c24`  
		Last Modified: Wed, 14 Apr 2021 20:52:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e82967ca9bc6ee6bdd75fdc4f9b9000c6fcb2c25b0d754591f4ea080d22c48`  
		Last Modified: Thu, 06 May 2021 23:36:04 GMT  
		Size: 105.9 MB (105944163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f7138aca5efa6f3f896323bc1d8d7e86ac97dc43934f657be7b59764fd1a93`  
		Last Modified: Thu, 06 May 2021 23:35:48 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1fc295bef09a7a41613606b2fab0bb9a2f237a924f638bbc1471e4cf7e8b91`  
		Last Modified: Fri, 07 May 2021 02:03:09 GMT  
		Size: 8.4 MB (8370195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e637a1eb5e336e7d0f477e2470ceb6a4501f134379834cd84e644993a10c733c`  
		Last Modified: Fri, 07 May 2021 02:03:08 GMT  
		Size: 1.3 MB (1264520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eeaadfe4374cccb5c1a67a72e18041ebe4ad77c344002126dc56db880377cfa`  
		Last Modified: Fri, 07 May 2021 02:03:08 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6e1481dcd1f0e4bbd49beb3bb38ce8a6846ee33a5630b1ca6af5e97deb6fd85a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.3.0-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:7c26382633835010d4cfd02b1c6fa418ce94cd4165e8eb946128fe754fc224c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2640840527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c7d48302374c8837dcb0b4a7eafbf5ab92ad9e14c7961978e4d6411547ce085`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:40:41 GMT
ENV GOLANG_VERSION=1.15.12
# Wed, 12 May 2021 12:43:35 GMT
RUN $url = 'https://dl.google.com/go/go1.15.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '313e5ebc59b497319c4c3f9560322fcc20f7bc3b4e47494afc3b2d63a42fb2a5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:43:38 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 19:53:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:53:05 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 19:53:06 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:53:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 19:53:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 19:53:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e10fb8a78b4fccaf2e1f27fade2351acbab7977f469077dbe3d61137a83bd1b`  
		Last Modified: Wed, 12 May 2021 12:59:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611233319702edb459b2c018bda3a84c557bdaed90507b5265b2802d845363c0`  
		Last Modified: Wed, 12 May 2021 12:59:39 GMT  
		Size: 134.1 MB (134130080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bae92e561d0c550e6481307d686ba1fd33b1c5ac6ea31411fb23e6db83b80df`  
		Last Modified: Wed, 12 May 2021 12:59:07 GMT  
		Size: 1.6 KB (1588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:206ea1b195825780737f5b6198def0bcdad5960c0341b1151836d1c07b9d2162`  
		Last Modified: Wed, 12 May 2021 20:05:37 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c2b185bf4960bb532474f7c1c09eed87a687f35127349952d45f9fbed859a1`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a954bd53bbccc7e000e23a03005396cf73110a1eef4cbb2b5713b094303abb`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b33214b7398e925aad6bb865e8c77d126584dec2ee7f66108665c4b2d407a57`  
		Last Modified: Wed, 12 May 2021 20:05:34 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a997270f53d496525fd665c09144ce7851254655d8651fdbb6f0d8b879a7c67e`  
		Last Modified: Wed, 12 May 2021 20:05:37 GMT  
		Size: 1.7 MB (1700479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57110530a8b452cb9ec0c7a6cefccc83019117e7d5477cb24669f1cde954240`  
		Last Modified: Wed, 12 May 2021 20:05:33 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:a1bc6a8c7f94c7315234c32c51f07caca9bd0e1bed11e24c65de50a5237af05e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:906461df38b01faa5b735a5c09cb4cebeed6d8edb2556dc81cc9dc80923146e8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5983275276 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b51d50a0e24be6c3ffc1c47427c3ce640d5e24f0e908ee635159d34278f463e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:43:55 GMT
ENV GOLANG_VERSION=1.15.12
# Wed, 12 May 2021 12:48:02 GMT
RUN $url = 'https://dl.google.com/go/go1.15.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '313e5ebc59b497319c4c3f9560322fcc20f7bc3b4e47494afc3b2d63a42fb2a5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:48:04 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 19:53:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:53:43 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 19:53:44 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:53:45 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 19:55:18 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 19:55:19 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e10c98a45913a3ce79e3502f8ad0b4a47ee36123faf47dcbf2795b50878648`  
		Last Modified: Wed, 12 May 2021 12:59:51 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8b9313f31970ae7f9cdeff1169da12a64965a580063923bf01a3f81af1b8c4`  
		Last Modified: Wed, 12 May 2021 13:02:38 GMT  
		Size: 144.0 MB (143977383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8b7390fa519672498ab6ced5bce95384a4922d59dbb35dd0725b1a6dedf33dd`  
		Last Modified: Wed, 12 May 2021 12:59:51 GMT  
		Size: 1.6 KB (1581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0a2adda3b5f16542c4a28642492806dd2009f6bc3032c3b9ef873715138d99`  
		Last Modified: Wed, 12 May 2021 20:05:51 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b9a511fdc0e9ddf64e9049876b9797f277670c797fa8839f5c4f623dc3558e`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90ade527b07762be1cffc2b787cc902d0f5836e4d75d3b745ecc24491769bab`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c752fd61bb0787576c60601f38f5ded35e90a6f86a39e72606bddeb9fb3603`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706f2f07a14a0961a5455784d51275ceaa6ad9ed410035c4b552ec7296fd0268`  
		Last Modified: Wed, 12 May 2021 20:05:58 GMT  
		Size: 7.0 MB (7042421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ae4915980d2bfd94575229474b5b9021fb64dc7781d5a14a075db51743e35c`  
		Last Modified: Wed, 12 May 2021 20:05:48 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore`

```console
$ docker pull caddy@sha256:49732c7d6a8a6d2d35a490d19e1b75f52b243ffc4579308e82d9b99b8d34d17e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.3.0-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:c7bcc9f9c51fc07386f4fe2a7b3dd9a5b8e1f0a5dd6f9422f80f67ed8fab2a54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.3.0-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1f2f4375fe18c3922246641f9d8147957d674518fbbae4de0ca7262ca9a10c8e
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491953956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81170266cc4cd4654c2a718b9ce95850c86f3d5007f3df0355cfd20ce5c88a8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:47:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:47:22 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:47:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:47:52 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:47:53 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:47:54 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:47:55 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:47:56 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:47:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:47:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:47:59 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:48:00 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:48:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:48:02 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:48:03 GMT
EXPOSE 80
# Wed, 12 May 2021 19:48:04 GMT
EXPOSE 443
# Wed, 12 May 2021 19:48:05 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:48:24 GMT
RUN caddy version
# Wed, 12 May 2021 19:48:25 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22448182e969b54b9124ea5c2c3274bb690098b2fbc33eb12e5ed9ed7050d5bd`  
		Last Modified: Wed, 12 May 2021 20:05:02 GMT  
		Size: 5.1 MB (5106938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94ef42ea7d797590afce1f67735ff57366d32b8e5a47fddd4eeba554353e1632`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6d6a870c119297feb4b26eb7ed0991f682ae7ed54eb6d078b3738540e4b07c`  
		Last Modified: Wed, 12 May 2021 20:05:03 GMT  
		Size: 12.0 MB (12036673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0306e9829e5a6249855c31f445349126971b770e640113282b8a295fc0903798`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c0da71a5fdf88e436b2eda07b3e01abd5e4980c4ff0df44058fcf7404d9d89`  
		Last Modified: Wed, 12 May 2021 20:04:59 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3abf7f593c565e5f425389811e406e60effd5aa026c589da05dda4e12a0e09`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af7361c77f2298946131dac665a1741fea61580de64d3720faf6bcad8bf6062`  
		Last Modified: Wed, 12 May 2021 20:04:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22941e833dbf1fbe60149b43d62e750e53f10b96fc0d3404f9f3557531f94c54`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de1004b1830150f2bfcf83cac0c69016d14353a11c98fc462bf6e09409fcc6`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86dd223159bafe127872fa6c79d7122fd5ef92ff99047ea461264d3bbdaffa3e`  
		Last Modified: Wed, 12 May 2021 20:04:56 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:616751d4c2002ece2f5f071e81f5ffb98eb13c9ccef5fc8d320763b236bd79fe`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e3d1e8fb9e4cc01652992548231f0624c9f312dc460e9c9bc6489b3ccaef13`  
		Last Modified: Wed, 12 May 2021 20:04:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7cd9649d7f83a1af93e815ee0e082bc07619910c657f910c373b76801a94afc`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2997645ef7e4b10b2f16f6574088dfed37540a6c331bdd818d19636cd0c288d0`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5329c49b05ecb4af421cd90b549f25d9d332ebd31e9c8c5caabe53e99cd511`  
		Last Modified: Wed, 12 May 2021 20:04:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab96feded9e3523c6bba4ca432a0ee98d1ed3058c81cc085615eb5676fa53a6e`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a1045f4017ab5a334bac615e62ee6d6849abba6b196cfdd731760f3fde0c23`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fee82082cb8928038f23a28f9132b659ac38d1bc6bb3afbc4e09dae54e86695`  
		Last Modified: Wed, 12 May 2021 20:04:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d0784bf95bc812b62f0220b913b05dd208b220f570884d7e34d7fcc0d37c4f`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 295.7 KB (295736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f43afb0cbdc146ba20b4aac840c48f5c77d4f58a4fdd0b6cfa0a45217f1bde75`  
		Last Modified: Wed, 12 May 2021 20:04:51 GMT  
		Size: 1.3 KB (1335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.3.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f73f193e59a09b16da5bcff4472514d0a9cd0c045457cfd4c1869f1f3f1f9441
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.3.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:9383b916fac221ad685d5162d3f13705bc54b48a8a4cc108c30bec9ebefccbb8
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5e85cd4236dadd2e2260e08847f06c7cf8a6bf114d46e5dc8d36a0624eb942`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:49:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/56302336e0bb7c8c5dff34cbcb1d833791478226/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:49:55 GMT
ENV CADDY_VERSION=v2.3.0
# Wed, 12 May 2021 19:51:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.3.0/caddy_2.3.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('afc504cb0a641729ba546c0cadea524a170dcca2a915473aaf032a7c666c7c56ac059752f34b5d50700a692647b9b395b530cd8299ac3650c729adce5daa1ba5')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:51:31 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:51:32 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:51:33 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:51:35 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:51:36 GMT
LABEL org.opencontainers.image.version=v2.3.0
# Wed, 12 May 2021 19:51:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:51:38 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:51:39 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:51:40 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:51:41 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:51:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:51:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:51:45 GMT
EXPOSE 80
# Wed, 12 May 2021 19:51:46 GMT
EXPOSE 443
# Wed, 12 May 2021 19:51:47 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:52:54 GMT
RUN caddy version
# Wed, 12 May 2021 19:52:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb86fc7ebd4b8e0170404d2efc422e3a003119cf835edf347cdba2cb5dcb637e`  
		Last Modified: Wed, 12 May 2021 20:05:24 GMT  
		Size: 5.7 MB (5715678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be0a1b98881464003a76f9c3d552af6aa32676eded40337a2cb740220b8e8b5`  
		Last Modified: Wed, 12 May 2021 20:05:22 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2f0820331f200b69ffc4376c6d900a0eff190f419b5000a08b1b2d643534b6`  
		Last Modified: Wed, 12 May 2021 20:05:26 GMT  
		Size: 17.4 MB (17386489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd3493d093c4b99f139a5427c673f7efaa2b5165503ecad87cb8ce5552e11ebf`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4fe562a331e468e75447f36e3f25418222bd38dd64ed86e1ed5d135326ca297`  
		Last Modified: Wed, 12 May 2021 20:05:20 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e380b48e44a8409c9d227325699b754573b99734b04ccd9b0afd4d221de4463c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4838e63e8d0097db4c9f0b40fb85cb4ca6ab86d367ba5e8e03926567a06fbf6c`  
		Last Modified: Wed, 12 May 2021 20:05:19 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8502433c7f52aac3dd7bda187871008ccc524909273d3ecc731fc21ae788d58`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436d7436a478513cfdd80519a071fb37badf42397c34e5bed6ecb807a0f5f544`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0957a349d9bda1d5d624590e5f8bb02b83605c041e63f495e421a185e7c9cb0b`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5368704288b662f01ec22e1518b4cbfbaebad0f096f0f78b523fbebf1bf8d315`  
		Last Modified: Wed, 12 May 2021 20:05:17 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97a57eac0f8fb22c77ed1133dce3b45ff210e67457237188fdd4244a614bcd9b`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06eb9e82c5d11b8714bdbcc16be6fef89cf5a8e80fa5aec957bb00ea13eb36c3`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b02b72008aedc5b17796c0bdc40233ae777ec8a19530b70983fa5b6f001914c`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e520b47523d14eb979eb9c33ee5803753ddf7192e0f9cc4737e596091333dc45`  
		Last Modified: Wed, 12 May 2021 20:05:14 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7cf16fae2c4e03aee1b9269abf928e7299c0912e8d6ce3c646b2398fd0419cf`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352e7ea39b707bbf4a83cc0c0be3ddf79f71be49669db9f93f17915d9e1235b6`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da84cbe314c1c929b4ce1e6c633c4e78b61d042c8ed8bcf96da263c53a1d12d3`  
		Last Modified: Wed, 12 May 2021 20:05:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d3810c939f9540e16a267e3d1f6a3e3e4162c5b6190d5087acc7eebdf65a014`  
		Last Modified: Wed, 12 May 2021 20:05:12 GMT  
		Size: 280.7 KB (280738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e6e97602e558f4a75b0da2af7de0ccca80cd60b809b803af3f16096fb85332`  
		Last Modified: Wed, 12 May 2021 20:05:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0`

```console
$ docker pull caddy@sha256:22f138ef9ab7e91e06e93e0a50de4cbddfa8519e6a3aeaa7abd09bb098996a6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.0` - linux; amd64

```console
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-alpine`

```console
$ docker pull caddy@sha256:0a3759d4e95e9af8a79858f7aa565d24ee8c2bf9a884faddcb1fe95d7ac52967
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-builder`

```console
$ docker pull caddy@sha256:2d9e7ddbd75ef569e39d2193b80d5c12389b9346943a24ab701ce3bc01b96983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.0-builder` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-builder-alpine`

```console
$ docker pull caddy@sha256:8b8beeef5c72efc27da7a1cdf0a8f816303907f9733c13386d25ebc6e7f785b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.4.0-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5f55710c6387a0a6e0562cac3d70bb758b2e8dd5ac30f84087c6eace39f32d98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.4.0-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f920c3ba405d271c71d4941cd7fd4007ea847358d7dbe13bb5f577bc53a4a281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.0-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-windowsservercore`

```console
$ docker pull caddy@sha256:ad9e5658ee462cc3b62a232aff6c0d10e99b6ac1542bb4ac859d1cbd8cb82cde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.0-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.4.0-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-windowsservercore-1809`

```console
$ docker pull caddy@sha256:99d81fbbaec988f2f6a5f961a1880bc32862547b81c458d55a224ca0830a2656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2.4.0-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.4.0-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:e6e167d7848926db64dc7882fdc689f69405ea5306161d6f5665a74358a7c760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2.4.0-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:0a3759d4e95e9af8a79858f7aa565d24ee8c2bf9a884faddcb1fe95d7ac52967
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
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:2d9e7ddbd75ef569e39d2193b80d5c12389b9346943a24ab701ce3bc01b96983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:8b8beeef5c72efc27da7a1cdf0a8f816303907f9733c13386d25ebc6e7f785b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5f55710c6387a0a6e0562cac3d70bb758b2e8dd5ac30f84087c6eace39f32d98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f920c3ba405d271c71d4941cd7fd4007ea847358d7dbe13bb5f577bc53a4a281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:ad9e5658ee462cc3b62a232aff6c0d10e99b6ac1542bb4ac859d1cbd8cb82cde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:99d81fbbaec988f2f6a5f961a1880bc32862547b81c458d55a224ca0830a2656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:e6e167d7848926db64dc7882fdc689f69405ea5306161d6f5665a74358a7c760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:0a3759d4e95e9af8a79858f7aa565d24ee8c2bf9a884faddcb1fe95d7ac52967
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
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:2d9e7ddbd75ef569e39d2193b80d5c12389b9346943a24ab701ce3bc01b96983
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:8b8beeef5c72efc27da7a1cdf0a8f816303907f9733c13386d25ebc6e7f785b9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:046f9aa5dcf83fb25e28e43539c520c8cd0dfe05faf14ad780826c7c36775145
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **116.5 MB (116541075 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd288b16c2ac5e35de34025c916a8a52cb8c3c35644e3e2beee860100beea6de`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:27:12 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:27:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:27:13 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:18:07 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:05 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:05 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:06 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:07 GMT
WORKDIR /go
# Fri, 07 May 2021 01:56:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:56:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:04:35 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:04:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:04:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:04:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adcc1eea9eeabb6de296adb3e0c1b0722cf13251ff3e4e2d0a5f7ed8e3d48342`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 281.3 KB (281269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4ab2625f07be8d5c6e48046a05ff3ecc7f374b794a926fb62247b66b511909`  
		Last Modified: Wed, 14 Apr 2021 21:35:06 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e7595549f7536d76f08a8a23fb67e3e6fae08ccf3add715c5c1c956f9445d2`  
		Last Modified: Thu, 06 May 2021 23:29:42 GMT  
		Size: 105.7 MB (105745828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df88182f7acff97ffde9f614a0fd86e8a26590e445aa76e442c3a79d9e4c4f4`  
		Last Modified: Thu, 06 May 2021 23:29:25 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d573d19fd03835237c7687f4f394fa6b1fc1c894a901f2853846256ee7746eb`  
		Last Modified: Fri, 07 May 2021 01:56:57 GMT  
		Size: 6.4 MB (6390123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95db25f5b69783a08df8902a5330daddf1e8b10bd1d8401b25d8f8ab43b6586f`  
		Last Modified: Tue, 11 May 2021 01:05:15 GMT  
		Size: 1.3 MB (1311169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74bfbae6287f60c1e9b89dd3e92e73d9f949ee6f11d78bc97a3e945ee20b2c68`  
		Last Modified: Tue, 11 May 2021 01:05:14 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:124237c870217e836b67b4697d7cddad2c3c58d50878dc51654db3605712c336
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.3 MB (112278566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15bef88e43f4622abd673fe82f110eb193559dd1abb2d8550178eb66032b4b5f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:00:55 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:01:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:01:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:24:09 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 21:27:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 21:27:32 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 21:27:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 21:27:35 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 21:27:35 GMT
WORKDIR /go
# Thu, 06 May 2021 22:10:19 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 06 May 2021 22:10:20 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:51:04 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:51:07 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:51:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:51:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:51:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4dea9fd179326b36ea137aad07e06571ffe7ad849e2a13a32354dcfd5d858d`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 281.4 KB (281379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeb04d84d23abf8470fc95982483a9117a87e55b13c591f5332a460a5233bb`  
		Last Modified: Wed, 14 Apr 2021 21:14:02 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26a3721aaa7ffedbec829a557c2d5f99c4661695a51f82632ece4df509b71bc1`  
		Last Modified: Thu, 06 May 2021 21:38:30 GMT  
		Size: 101.9 MB (101925593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298c78bc6b40a671a2f9a64d2cecf253acd10da30924ff687012e02b0307a1a8`  
		Last Modified: Thu, 06 May 2021 21:37:54 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3d237d41fc2805c9d9a047d4bb2618233c7093cc31d682b5231e0261a8c201`  
		Last Modified: Thu, 06 May 2021 22:11:03 GMT  
		Size: 6.2 MB (6227066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ffbb7f2dd65c638ffd56b2ab5964193545041922501d15451a2b6f4b0b0edb`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 1.2 MB (1221678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d30db79a4a633e8984befac9884a645ed6f3bd581f677daa8a26f2cbda65a4`  
		Last Modified: Mon, 10 May 2021 23:51:50 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a4ecc2040cdcc0166a3fea577c4e704d291fe70c2c65c460ff347d06c2b54046
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111227459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d2c6dfa3a578099a3e909c80cd793b780fb7a9135d5f28ec25270157a0902f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 21:00:38 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 21:01:31 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 21:01:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:11:51 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:15:25 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:15:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:15:28 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:15:29 GMT
WORKDIR /go
# Fri, 07 May 2021 02:34:14 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:34:14 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:17:54 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:18:06 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:18:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:18:32 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:18:34 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb6bd423db0b63fdc83c72eae7ef401cb2fb9eaa63961c71a867ff26bfe422f`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 280.5 KB (280532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835b667ae68ff940439602ffbabae6e923c687cb56c62a793f23ddca67584049`  
		Last Modified: Wed, 14 Apr 2021 22:44:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5b93a32354ff48887c2e9c4540875b8aa57822ab5c261d95e3c186d27b5c5e`  
		Last Modified: Thu, 06 May 2021 23:28:23 GMT  
		Size: 101.7 MB (101743890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2925b4cee8520caf8150ba3410d1306c50fa326f2fd920488f9e432578fda5`  
		Last Modified: Thu, 06 May 2021 23:27:52 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc435726a63967cbbe522309fca3524e0e1fd01e955717cedc9e172d632cbd1`  
		Last Modified: Fri, 07 May 2021 02:34:54 GMT  
		Size: 5.6 MB (5558665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd402931cf263713336d2aa524723f4caec26b90c0d6406651b14a2f88a642ab`  
		Last Modified: Tue, 11 May 2021 01:19:24 GMT  
		Size: 1.2 MB (1219508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee3295bff1b446bc98e483336ce527bcd52ccfecd1930eba95c70c26e909f3a`  
		Last Modified: Tue, 11 May 2021 01:19:23 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a8418ff913feb35632b8e2e0e2dde138632b289047de19713b0c24fe65c6eecc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111763060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68622e818b4c271dd7faf093081a9641f809d407eb6dc67bb6afe822393b4b0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:40:18 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:40:49 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:40:55 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:31:41 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 22:33:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 22:33:53 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 22:33:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 22:33:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 22:33:57 GMT
WORKDIR /go
# Fri, 07 May 2021 01:17:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 01:17:19 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:40:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:40:21 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:40:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:40:25 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:40:26 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7186ed65a4f7bb0e9cd4b00f43359b47a4f19749dbd48e704fc578a4f43d7c96`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 281.5 KB (281488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:316046926c0ae5f42710c1197ed3de9fc374986179c18611f523cf4521adeef1`  
		Last Modified: Wed, 14 Apr 2021 20:59:32 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:696a969ea94b7c2e3938ec670b72c32f58ece636bb7ec6526d0efab40e760bce`  
		Last Modified: Thu, 06 May 2021 22:44:20 GMT  
		Size: 101.1 MB (101090590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff4d3f41a5567d10cda7e4f3c4267dbb9181eb63bb52c950c3dce3327a9a36e`  
		Last Modified: Thu, 06 May 2021 22:43:56 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec12dccc6ac2c5238a0e958e58c89d37f56cf2e181ba8a4f291b176a2a20fa`  
		Last Modified: Fri, 07 May 2021 01:18:00 GMT  
		Size: 6.5 MB (6476691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803dba8659a2ec5c5a177383797832eca7c7d301ec4253e47ee42527aa617bac`  
		Last Modified: Mon, 10 May 2021 23:40:59 GMT  
		Size: 1.2 MB (1201547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e70f326991067a04529de021321ce20d6920e81d14aaef93afb92136c976508`  
		Last Modified: Mon, 10 May 2021 23:40:58 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:58ffe092c4ccbd15cf9faf25d63caa632bb639d53188a377038834ebf2dac85a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110621059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2321e3937c686734c8c9124a34811d9eb4092b7611145be19ea453a5bbb389a4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:53:57 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 22:54:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:54:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:22:47 GMT
ENV GOLANG_VERSION=1.16.4
# Fri, 07 May 2021 00:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Fri, 07 May 2021 00:25:26 GMT
ENV GOPATH=/go
# Fri, 07 May 2021 00:25:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 07 May 2021 00:25:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Fri, 07 May 2021 00:26:14 GMT
WORKDIR /go
# Fri, 07 May 2021 08:19:51 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 08:19:57 GMT
ENV XCADDY_VERSION=v0.1.9
# Tue, 11 May 2021 01:19:13 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:19:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 11 May 2021 01:19:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 11 May 2021 01:19:30 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 11 May 2021 01:19:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf726c40dc4802009a4b6f0f7947c86242c2c078623e8f1f21343864093b3a9`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 283.4 KB (283413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c17712dac96942b05a27f88ea5346bd57b4cabdb33c153562ef144635225b3`  
		Last Modified: Wed, 14 Apr 2021 23:05:31 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d2e93731067b7b48232c826d062ff4fead572dbd98e0a28642db4802342a8e`  
		Last Modified: Fri, 07 May 2021 00:41:39 GMT  
		Size: 99.5 MB (99528032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca0e521f95ca5f22fdd4b7917d06aead7df46288885c4fd3ffac0242b96643f`  
		Last Modified: Fri, 07 May 2021 00:41:14 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d9dfa7e81a349fea3e170fbc6f6b9fd3245ee43c53b329a3ae72c9e5ebaddfb`  
		Last Modified: Fri, 07 May 2021 08:22:18 GMT  
		Size: 6.8 MB (6825232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e87f3bfd07b70b357098f4ba50744bf3c838e8c3ab709598b79864f29b676311`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 1.2 MB (1170526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68dce6545308f135393f568603954610d88f7a8a61ca402820d75500d925926c`  
		Last Modified: Tue, 11 May 2021 01:20:23 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:e72252e76203d04b2ed847e26d71ca0de7ed89c2d76990ac177fb80755d88617
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115474412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b08b1e73df9c564bfdb9249c0d32c47642dd69cd88bfa280b4682767ef8fe671`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:45:11 GMT
RUN apk add --no-cache 		ca-certificates
# Wed, 14 Apr 2021 20:45:11 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 14 Apr 2021 20:45:11 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:16:38 GMT
ENV GOLANG_VERSION=1.16.4
# Thu, 06 May 2021 23:20:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		bash 		gcc 		gnupg 		go 		musl-dev 		openssl 	; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		'x86_64') 			export GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$apkArch' (likely packaging update needed)"; exit 1 ;; 	esac; 		url='https://dl.google.com/go/go1.16.4.src.tar.gz'; 	sha256='ae4f6b6e2a1677d31817984655a762074b5356da50fb58722b99104870d43503'; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC EC91 7721 F63B D38B 4796'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		( 		cd /usr/local/go/src; 		export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 		if [ "${GO386:-}" = 'softfloat' ]; then 			GO386= ./bootstrap.bash; 			export GOROOT_BOOTSTRAP="/usr/local/go-$GOOS-$GOARCH-bootstrap"; 			"$GOROOT_BOOTSTRAP/bin/go" version; 		fi; 		./make.bash; 		if [ "${GO386:-}" = 'softfloat' ]; then 			rm -rf "$GOROOT_BOOTSTRAP"; 		fi; 	); 		apk del --no-network .build-deps; 		go install std; 		rm -rf 		/usr/local/go/pkg/*/cmd 		/usr/local/go/pkg/bootstrap 		/usr/local/go/pkg/obj 		/usr/local/go/pkg/tool/*/api 		/usr/local/go/pkg/tool/*/go_bootstrap 		/usr/local/go/src/cmd/dist/dist 	; 		go version
# Thu, 06 May 2021 23:20:18 GMT
ENV GOPATH=/go
# Thu, 06 May 2021 23:20:18 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 06 May 2021 23:20:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Thu, 06 May 2021 23:20:21 GMT
WORKDIR /go
# Fri, 07 May 2021 02:02:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Fri, 07 May 2021 02:02:35 GMT
ENV XCADDY_VERSION=v0.1.9
# Mon, 10 May 2021 23:42:03 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:42:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 10 May 2021 23:42:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='8b36aa88d294cfd47e2bbba24d99559a5327db84de0a0b3c28e9f2c8e7c9df16bef96ca0cf033e6304474b7d94336843ee9665bf5159815ecac7986e3ee508bf' ;; 		armhf)   binArch='armv6'; checksum='7f8711d98e42ab6fb96fd7405df34944bcc97b16eab7c3d45fd8b496f690bed5cf041cc694b5b615fd88f91e87f75995501c484021f0d510b61375b6888efcc5' ;; 		armv7)   binArch='armv7'; checksum='adf762a2c765c84a933ad2b1b27609f3bf1b2394587cd9b199c661b02eea8783a7910b4dced1f8fd6bd33761a7ca792e1328f6acf54d9e4772922d095e541709' ;; 		aarch64) binArch='arm64'; checksum='4b914ffb89e0cacbac3d2dcf8e0db4682939d27d64160191f6941ba80dbb439e4d06d511ec6fefd1969a51895cdbd7b10dc0737efb13250ce9a03b39ae5cc6d3' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='e4bd087f7e9df1973af14fc420211976cdb34111349d36ad5e1bc193312bf076fc9fad8ce58ebdf09f9d7ff94017ce9dbab7c10fea1c0719ca26b9dc0cac5559' ;; 		s390x)   binArch='s390x'; checksum='4e2d075a0fa326683a4911dddcd0776f9de828645c602b9cdf1a6998c438ef265b6d4bb1ce85ef14de2064d7b2d730d36220fdff231674d67df33205ff3eec0b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Mon, 10 May 2021 23:42:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Mon, 10 May 2021 23:42:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc746875ae346ee6ec3c9080f8a7a50bef3899ea9d5ae9dac45a81bfe861c9d`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 281.7 KB (281708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0242688236000dd8f33d16f89f36da3ef1bb2a7a32bb59a7eb97a18ed3d5158`  
		Last Modified: Wed, 14 Apr 2021 20:52:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dab17b6808078a43afd3d62f1a202857192406e914c33d5ceb5eec1eb05eeb`  
		Last Modified: Thu, 06 May 2021 23:34:08 GMT  
		Size: 104.8 MB (104849388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6059cb089a1bd1108012ddff056f297d814995f95d29d57b15c13d11baede00d`  
		Last Modified: Thu, 06 May 2021 23:33:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84919c1c43955cfb518f179d4f6b541cdfa94579f6f6ef10fdc6e6b3ca4d51a3`  
		Last Modified: Fri, 07 May 2021 02:03:18 GMT  
		Size: 6.5 MB (6475416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3025f5e46ec68c9ef05a49a22ca89718a0d154f401122b0505a18d1c9217fc`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 1.3 MB (1264531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19bb5d9c7e67f1492e82b3f7c19e6900095d43b1f65fa5496f752a95169cd953`  
		Last Modified: Mon, 10 May 2021 23:42:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:5f55710c6387a0a6e0562cac3d70bb758b2e8dd5ac30f84087c6eace39f32d98
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:67216c69a5c02a4184c215f69d5303c90eae5e26ac1457152d5e007f72fec0c2
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2646051118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:915b4be5db3db4ad105d028bb9011b8eba0999fd9ae0152f2e40f94d30d2068b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:24:28 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:24:29 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:24:30 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:24:31 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:25:34 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:25:36 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:26:02 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:26:03 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:28:52 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:28:54 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:01:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:01:39 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:01:40 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:01:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:02:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:02:09 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2a5ccd12170e9f926c3e069a2fa2ed38b5dd5596869ed982bccc50ef80cf1f`  
		Last Modified: Wed, 12 May 2021 12:52:10 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd5b5fa12081ad53ae688dc454e550dd50bd414c949724180719b0326632c4a`  
		Last Modified: Wed, 12 May 2021 12:52:08 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599ef939f9e7c26d4bc0f8f75820116f6977a64212b86260bc225ae2d850cc31`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bddce42b6f4351510fcb255839a7c55d95546186dce8509782abe959d27d9f0`  
		Last Modified: Wed, 12 May 2021 12:52:07 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2407bf3b614294860b53b94e661f5c57f7dd985934aed5727442f9353bf8c617`  
		Last Modified: Wed, 12 May 2021 12:52:14 GMT  
		Size: 30.2 MB (30189126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b01ea9b4210c3201c1462d7ee78b276d7d5ffac3dca02c9c57a0c77c5b87a2`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27be8fd19f331f65055bbf31138aa28628be7534753008620ec14fc1803ebdf2`  
		Last Modified: Wed, 12 May 2021 12:52:05 GMT  
		Size: 313.1 KB (313094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421c063618ce27e648851fb286affe0950f7139e757b3df32c000a57be356623`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a33f0b9cbc9b02b55024fe76b7bac201d2b1037026b89c771078012fd84461`  
		Last Modified: Wed, 12 May 2021 12:54:46 GMT  
		Size: 139.3 MB (139340646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0884ee5b71061eefa8cabccdfeea059b656359a6ebc477d6f43284bccbd2057`  
		Last Modified: Wed, 12 May 2021 12:52:04 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388dabb05e13f4119ef08ddb7ab1531da945ae5934f70bf1ead828148c77e9b0`  
		Last Modified: Wed, 12 May 2021 20:07:41 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39998044c69992575089510bbe2da6af14ac95b838cdd6ff78ded4896c641cb`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0725d3d7bce7943a844847e6c04ea424d0d2990f701035df72fb6d5e51138e`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc021721ce1cfd67fb8ff246d57c2116ee4f3637820bc5c9031bf2490c2be341`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cee199bfc5e8edcb366243b91984a10b873843202a629d3cb03c799f766817a`  
		Last Modified: Wed, 12 May 2021 20:07:40 GMT  
		Size: 1.7 MB (1700522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a16a090b6e01c9dc03c57fc89b63671d071df752824b7095031573e56794a18c`  
		Last Modified: Wed, 12 May 2021 20:07:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f920c3ba405d271c71d4941cd7fd4007ea847358d7dbe13bb5f577bc53a4a281
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:builder-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:3fd63e42cd0402f5c3c52d35aecc68abd19a6e5ddbdff6f77446e1fbc91c6ecc
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 GB (5988473266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed74be70e20ca641123204f86b72459f3e650475b3fa997ca9339391a921c947`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:29:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 May 2021 12:29:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 May 2021 12:29:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 May 2021 12:29:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 May 2021 12:31:44 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:31:45 GMT
ENV GOPATH=C:\gopath
# Wed, 12 May 2021 12:33:10 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 May 2021 12:33:11 GMT
ENV GOLANG_VERSION=1.16.4
# Wed, 12 May 2021 12:37:08 GMT
RUN $url = 'https://dl.google.com/go/go1.16.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'd40139b7ade8a3008e3240a6f86fe8f899a9c465c917e11dac8758af216f5eb0'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 May 2021 12:37:10 GMT
WORKDIR C:\gopath
# Wed, 12 May 2021 20:02:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 20:02:17 GMT
ENV XCADDY_VERSION=v0.1.9
# Wed, 12 May 2021 20:02:18 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:02:19 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 May 2021 20:03:44 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.1.9/xcaddy_0.1.9_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('d03d5f6e22cc1c7dfbfd7ca0946a1c313e6b7cf24eb846b4a732452445cede8ec1a3caff6d78b4ba6a47f8dfcfc85d989beb1165e5b74c230eabb0d20a3c6379')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 May 2021 20:03:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10abf429e12c7b3b7d2b0a791d7cdb47866461a7b63df4ddd4f63acc91e26231`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79955f676504cbf77ec284d8e857d18d17b93c5b8e6438b4062dd80f8632c9d6`  
		Last Modified: Wed, 12 May 2021 12:55:12 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24af485ecab19f81a0c65c0eaec6f6fda8749ca50eb53101abcfc5c079f9b1c2`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b782f6bcd162ee81518d73c6c4fe5c5b731ab38b595c16a55ac185db84b2c9b`  
		Last Modified: Wed, 12 May 2021 12:55:07 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1327fc384f9fff64d41446adcb3bdf585307370ef0024a31a5269bae6f30067d`  
		Last Modified: Wed, 12 May 2021 12:55:18 GMT  
		Size: 30.8 MB (30797956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1c50f4b0b5994b4154be9fea2ab6c6a0e4c402c44d44795a5ce82ab6f8de4bc`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e458669a58e08411a0641a721ef1daf4af2a568c4dd61e9a3710b07f73b6ec`  
		Last Modified: Wed, 12 May 2021 12:55:13 GMT  
		Size: 5.7 MB (5661591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d753db33d9475a781a71db67226b6c2805f1e71108748b94dfdd610bb33137d`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16cf5cfefdc254a6ea68d79ebf521696de46090dd4d38c207ff2e301ff621d2`  
		Last Modified: Wed, 12 May 2021 12:55:48 GMT  
		Size: 149.2 MB (149178430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8924854b0100f624a921d0d3d2922ca97fd7cca3d49cdc1dd677d10f628a122c`  
		Last Modified: Wed, 12 May 2021 12:55:04 GMT  
		Size: 1.5 KB (1543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3d1201ff9263b27c3203fb740b420dfc811d03d441859aefe187732f9f4f54`  
		Last Modified: Wed, 12 May 2021 20:08:00 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7ea4eae8e32e10e3ec07876a089c1bc058b7360f4cbe858bb6555f86da0b198`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdd5be6e64ffa6a28903d7bbe1625e9868549d876d6bb16a443076ca9b947b0`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a86c894882db72f9825f01024eeafd6727ee19b893680e6ed68afe302582330`  
		Last Modified: Wed, 12 May 2021 20:07:57 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9a977d17c44f8027cef7906437f5950545fe731eb4842c3fe230d62541eaf3`  
		Last Modified: Wed, 12 May 2021 20:07:59 GMT  
		Size: 7.0 MB (7039449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6270ebfaadfbad9a78441cd8a19d2e9efcc162e2e7d382f624c0f6276d5b32`  
		Last Modified: Wed, 12 May 2021 20:07:58 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:22f138ef9ab7e91e06e93e0a50de4cbddfa8519e6a3aeaa7abd09bb098996a6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:6395c0a4bfcc76ccd72e0c77bd609c3561f941a32321456520357a278dd113f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14566627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c76f8655142c3788bcce68be571bdc12a9eb162cbef12a8b0cd9828e80ae62f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:11:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:04:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:04:24 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:04:26 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:04:27 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:04:28 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:04:28 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:04:28 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:04:29 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:04:30 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:04:30 GMT
EXPOSE 80
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 443
# Tue, 11 May 2021 01:04:31 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:04:31 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:04:31 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8294633c5b5606f8e98aaf81da701b7a7e2018dbf82355d1d73830c677034f19`  
		Last Modified: Wed, 14 Apr 2021 20:12:08 GMT  
		Size: 300.4 KB (300403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16798e0582fce7af9c2ba2c8ee4990d0fd1e58384e170ee9937486253d67bbf1`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc7caf536ee3257ee5085ea50b1fdb2342f1ba7cf67dd718c14657bc29c9c1df`  
		Last Modified: Tue, 11 May 2021 01:05:02 GMT  
		Size: 11.4 MB (11448248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55d296ee3d96b0a8ddf81c22c5416bfdfb98b4e987079dea3f1d2a407a0a3d7`  
		Last Modified: Tue, 11 May 2021 01:05:00 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:accd51f67c4da65e48a62067231d7f279a7414c84f7e3a074ea484a8024e7ddf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.8 MB (13781937 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e539d0aea8e90bdb3c7929a807a5300f0e2ad19de1a5eea2b7307a99f573271`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:46:41 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:50:08 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:50:20 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:50:28 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:50:32 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:50:33 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:50:34 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:50:35 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:50:37 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:50:38 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:50:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:50:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:50:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:50:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:50:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:50:46 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:50:47 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:50:49 GMT
EXPOSE 80
# Mon, 10 May 2021 23:50:50 GMT
EXPOSE 443
# Mon, 10 May 2021 23:50:52 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:50:54 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:50:55 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf1089ae45174c5bef4f470e0e4c2337f99090005f19e104781d0b048ea9c3b`  
		Last Modified: Wed, 14 Apr 2021 19:48:05 GMT  
		Size: 300.5 KB (300511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c14f76d7a7af16ae081f310cdc4fedb50982a53c62946c7880f5333bd47c28`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 5.8 KB (5850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f575ba8a69ca1a5904bf22dad27c7546342af53febbc35ccb5dd267e8feab97c`  
		Last Modified: Mon, 10 May 2021 23:51:43 GMT  
		Size: 10.9 MB (10853292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c324d5c3633091e7997d13f43fe84f9ac2bf7794d197fa229113ad4c902faf2f`  
		Last Modified: Mon, 10 May 2021 23:51:39 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:159edc693b6f3d45e04ab7307ea31bfa442d06231b69e5f42bff5eb2125ab1fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.6 MB (13559369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfb4539c52fe67844a8b90b8d3a0bf118a6896f043571a3a8d6218cdb32f69b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:40:17 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:15:41 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:15:43 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:16:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:16:43 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:16:51 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:16:52 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:16:54 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:16:55 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:16:57 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:16:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:17:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:17:02 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:17:04 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:17:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:17:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:17:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:17:12 GMT
EXPOSE 80
# Tue, 11 May 2021 01:17:13 GMT
EXPOSE 443
# Tue, 11 May 2021 01:17:16 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:17:19 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:17:22 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f77b739097bd5400613d0daa0adde01d99993ce236a374da6748f11f866bf0`  
		Last Modified: Wed, 14 Apr 2021 19:41:38 GMT  
		Size: 299.7 KB (299662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5d4f3a32ad0ee5557140984ec66d8aec7518580e0b4f25075abc467852f5c9`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c575185c831e1739dc7ab125ed53c9c9eeb2d30e22cf98463c504b37032eaa50`  
		Last Modified: Tue, 11 May 2021 01:19:08 GMT  
		Size: 10.8 MB (10829560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaaca182d4fd03b56b6b3a42f2291ff209334224c854363a79e5ebab993f3230`  
		Last Modified: Tue, 11 May 2021 01:19:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:a7b0a04a662cf260a34977b125179056a62db0b2e1851c1dd7d8ebc9f8cfc759
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.4 MB (13415216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f513d5a7342c2d3b29180971441798c54e90a4bae8566531b9ad22ed40df6212`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:47 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:39:51 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:39:52 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:39:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:39:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:39:59 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:40:00 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:40:01 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:40:02 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:40:02 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:40:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:40:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:40:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:40:06 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:40:07 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:40:08 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:40:09 GMT
EXPOSE 80
# Mon, 10 May 2021 23:40:10 GMT
EXPOSE 443
# Mon, 10 May 2021 23:40:11 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:40:12 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:40:13 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0e0200fa31a158cd37e4584ab7ca30d0663376cf38fe7f1b73ff5a9a59fa12`  
		Last Modified: Wed, 14 Apr 2021 19:02:06 GMT  
		Size: 300.6 KB (300628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7a226e39f1950acc413ed3ac67a7b336554ce3e8b6f18944919ead2f26fc64b`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 5.9 KB (5852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4960f1f64846804fc30f5058d85051d76e307a619fc59284272e71e7499c3a38`  
		Last Modified: Mon, 10 May 2021 23:40:51 GMT  
		Size: 10.4 MB (10396556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f958efe8814c77472d3cc7966c7cd904e5d478ebb7a6bc55787ec52ed29cc6`  
		Last Modified: Mon, 10 May 2021 23:40:48 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:d211f951fe7f23617be7c14d71ed0cd4119eaab14cbf966986edc416f0c0be82
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13116860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd138e3e0b764e1303127c59ea74d320008abb27509713e2e0cdd44a2354978f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 22:12:15 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 11 May 2021 01:17:01 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Tue, 11 May 2021 01:17:09 GMT
ENV CADDY_VERSION=v2.4.0
# Tue, 11 May 2021 01:17:23 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 11 May 2021 01:17:40 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 11 May 2021 01:17:48 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 11 May 2021 01:17:55 GMT
ENV XDG_DATA_HOME=/data
# Tue, 11 May 2021 01:17:59 GMT
VOLUME [/config]
# Tue, 11 May 2021 01:18:03 GMT
VOLUME [/data]
# Tue, 11 May 2021 01:18:09 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Tue, 11 May 2021 01:18:13 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 11 May 2021 01:18:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 11 May 2021 01:18:20 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 11 May 2021 01:18:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 11 May 2021 01:18:27 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 11 May 2021 01:18:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 11 May 2021 01:18:40 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 11 May 2021 01:18:46 GMT
EXPOSE 80
# Tue, 11 May 2021 01:18:49 GMT
EXPOSE 443
# Tue, 11 May 2021 01:18:52 GMT
EXPOSE 2019
# Tue, 11 May 2021 01:18:56 GMT
WORKDIR /srv
# Tue, 11 May 2021 01:19:00 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25908330df11bb7bc2ed71aa9b4de279db5492df2b03ced3f6650b25821c4584`  
		Last Modified: Wed, 14 Apr 2021 22:16:00 GMT  
		Size: 302.6 KB (302554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a224581e3ba4733f37686f5a5d5375019f9126a0ded6ed20f13e09e898dc735e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 5.9 KB (5853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd74ee5b1b1729043f41d60aef4d52f55ec9f64d89cd625caaf037ae0c7be6`  
		Last Modified: Tue, 11 May 2021 01:20:11 GMT  
		Size: 10.0 MB (9995159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e0bfaf16f0b56abead39bc99d52694122454078fb2e2e9e29f4209f4daf0a8e`  
		Last Modified: Tue, 11 May 2021 01:20:08 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:9e5a00e41c90ba5e0300a6397166cc06dcfac524c3221fa520a9ded1ce6c163b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13937005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adc589ef8ecca20bb3a9cd3b06f370d0f4c74397fc459cf6cf14588d7d0c64c9`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:07:40 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 10 May 2021 23:41:38 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"
# Mon, 10 May 2021 23:41:39 GMT
ENV CADDY_VERSION=v2.4.0
# Mon, 10 May 2021 23:41:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd6427ba877d286f5af229e439e59a05afe840283c7674589f46a3bd2bcb25f2162295d55c705f052318a85de23f3661f8322628e952cc1a0f784a8068f68357' ;; 		armhf)   binArch='armv6'; checksum='088f011a1e71fa3312b907bcdcfe545ba69294e3310acdcccf453c7096498dd61bb818cd19e1fca164711e878a662965bcbfd9946574a20403f71711537a76de' ;; 		armv7)   binArch='armv7'; checksum='32fe7ff1544e3845b181fadd394383f31522239476f7df031f048856ec3ae73264f70eb3934e6074b7bba385e1188cacef6b7c941e80b1f9a303711eecae396b' ;; 		aarch64) binArch='arm64'; checksum='2c4fa4ce1465e1dc8e97d669bde9df50a06f4c21a916e59d32d5a4af7be449fc3f0f18303e43ff95655202832898bbdf02148b4aaa1e9e205d487ef14482b31e' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='1ab37dba5fea5e55a403b51d59faa1d4ba74eb3065584fdf585562ae88de6396b5296e5d3c107e5bd2a08cc4e77dce2a8ee29f291a5d4639b4a097b47de9dbf9' ;; 		s390x)   binArch='s390x'; checksum='ec9319f3ade6ead60c2b6c1a8c5649ca6f911efef938970fc1f08a613ecf9d582b507aad178a7c75fdcf502164cbf4f4563553c40be2ced529c6b0844def8341' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 10 May 2021 23:41:45 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 10 May 2021 23:41:46 GMT
ENV XDG_DATA_HOME=/data
# Mon, 10 May 2021 23:41:47 GMT
VOLUME [/config]
# Mon, 10 May 2021 23:41:48 GMT
VOLUME [/data]
# Mon, 10 May 2021 23:41:48 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Mon, 10 May 2021 23:41:49 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 10 May 2021 23:41:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 10 May 2021 23:41:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 10 May 2021 23:41:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 10 May 2021 23:41:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 10 May 2021 23:41:54 GMT
EXPOSE 80
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 443
# Mon, 10 May 2021 23:41:55 GMT
EXPOSE 2019
# Mon, 10 May 2021 23:41:55 GMT
WORKDIR /srv
# Mon, 10 May 2021 23:41:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3c8b812fcb0d1bfd42c16c2e9ac68f4f3006382c5362e969d1c9eb3a9fab5`  
		Last Modified: Wed, 14 Apr 2021 20:08:26 GMT  
		Size: 300.8 KB (300847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eba030675d7bb5bc251d93896d2c81ed8a2f4f4ef2e8e84ad7dfdce9886387c`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 5.8 KB (5847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645cac8e572aad7be24e99df8012056e9752654f6923bf19b08171139a76793d`  
		Last Modified: Mon, 10 May 2021 23:42:31 GMT  
		Size: 11.0 MB (11027506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d6ae883db75a7ce02c9b38976d8aa73fe94d35701ce4f589302e33cc88710d`  
		Last Modified: Mon, 10 May 2021 23:42:29 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:ad9e5658ee462cc3b62a232aff6c0d10e99b6ac1542bb4ac859d1cbd8cb82cde
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64
	-	windows version 10.0.14393.4402; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:99d81fbbaec988f2f6a5f961a1880bc32862547b81c458d55a224ca0830a2656
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:6c90801f6bfb64f1b15c4d4aa94fcff5c97fc51849c0387bca0dd172d2eb193a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491813719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0704966e32c02181cb99b42655a02dc072fda4af8e0f3e994c8ed03bca51397`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:56:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:56:09 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 19:56:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 19:56:40 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 19:56:41 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 19:56:43 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 19:56:44 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 19:56:45 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 19:56:46 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 19:56:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 19:56:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 19:56:49 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 19:56:50 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 19:56:51 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 19:56:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 19:56:54 GMT
EXPOSE 80
# Wed, 12 May 2021 19:56:55 GMT
EXPOSE 443
# Wed, 12 May 2021 19:56:56 GMT
EXPOSE 2019
# Wed, 12 May 2021 19:57:15 GMT
RUN caddy version
# Wed, 12 May 2021 19:57:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dc51194378204d7114732c3ee4da8d6b390b048e70ae1535a082de3ff67b5c`  
		Last Modified: Wed, 12 May 2021 20:06:24 GMT  
		Size: 5.1 MB (5106604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8351dcfe8a845de2e6479ec4f32c51bb12b153b902cb5c2bb82609c41f1ee2d4`  
		Last Modified: Wed, 12 May 2021 20:06:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77c18e7f054169630e570665848653b24c46b6a00a683762b47af6395baf40a`  
		Last Modified: Wed, 12 May 2021 20:06:18 GMT  
		Size: 11.9 MB (11896492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d8483c175b501eba292fef2d8eed1fb175da233f42e5b8a29731d16e2a473f4`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7668bdbd1be65f36a3957829a164c943fb88e2d66fc86110d2463c96e6429c4a`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a223eedc30f76e71d9f308b679af48d45ddb6b1d9bf351dbc6cfa2b91b1baef2`  
		Last Modified: Wed, 12 May 2021 20:06:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3c724ddef04ed3db6561a26b394ff76c603f3dfcf7348844290006c954c9ab`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a613a41808979c676171c90f63a505cb2ff23e33230c7317e0cd926f6f70e`  
		Last Modified: Wed, 12 May 2021 20:06:12 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c55f8cc0bde2e5ccde5ebd8620809311b4842385f747b23a9c69fd30ad1450`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bd5b8a97f52a81d458eb8ffdee258f25ae63ef501eb36f92af1a87ecf9c3dc`  
		Last Modified: Wed, 12 May 2021 20:06:11 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34fd7860cad12e325fa5abe4bd5e1938322a83967a7f6de263a0e0f24eab8efe`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b2d0d7f697498b318b3588b629e5e5312077292c3e69b5db77d45fc106917b`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31440ce7a4b62f8d172fbbf5d73f8376372db8fd6606daf040a522ce10644f42`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67029fa2eee16b2a9cd9bb479534c8c861a33c5bda5fdc0e13eca4fb1559b69d`  
		Last Modified: Wed, 12 May 2021 20:06:08 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513cef3a4f0e5872a6dff98edb78b885e6cd661e51392ead0f87127cc47906ca`  
		Last Modified: Wed, 12 May 2021 20:06:09 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92481bb3076fd22988205dbb34e7dc4baf1525f5da164223362a23359398472c`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c36a79c2d1000c4f4a6d0c0ba9e97848cafb854dff9fd583178ebddd9ad9bcd5`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:806e48d3f423d032d3c9d11c520f30035ad53f34888eaf6a83f9dba40cecb476`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d47bf5a474f4bef33b69317e6acc971a57f081ad5bba147e2aa9142aef662d`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 295.9 KB (295874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:741fcb5f17532b897086a6c7b00585a1d78abd8bc20d3c872e868ff7a3e38ead`  
		Last Modified: Wed, 12 May 2021 20:06:06 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:e6e167d7848926db64dc7882fdc689f69405ea5306161d6f5665a74358a7c760
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `caddy:windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:838ae0adcb062de173e145d0796c15d6fb9bd9c336b76162ead2e187d2774083
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819049733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639aa79ba7fccaa86390dac55ea0a3b3015deca7f880237c3260907aae4a9e4d`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 19:58:49 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 May 2021 19:58:50 GMT
ENV CADDY_VERSION=v2.4.0
# Wed, 12 May 2021 20:00:20 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.0/caddy_2.4.0_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('66c1f96e5ceb44aec53727ec02bbbb52eb58b4a41ac1134c5635693f40aa81cc4fa8e5418fdf712c8aa9c710aa0b19d6f52c0b46c6af54b4c79ca602e599694a')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 May 2021 20:00:21 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 May 2021 20:00:22 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 May 2021 20:00:23 GMT
VOLUME [c:/config]
# Wed, 12 May 2021 20:00:24 GMT
VOLUME [c:/data]
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.version=v2.4.0
# Wed, 12 May 2021 20:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 May 2021 20:00:28 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 May 2021 20:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 May 2021 20:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 May 2021 20:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 May 2021 20:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 May 2021 20:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 May 2021 20:00:34 GMT
EXPOSE 80
# Wed, 12 May 2021 20:00:35 GMT
EXPOSE 443
# Wed, 12 May 2021 20:00:36 GMT
EXPOSE 2019
# Wed, 12 May 2021 20:01:29 GMT
RUN caddy version
# Wed, 12 May 2021 20:01:30 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c26858854e9a4d33437022a0cbf481973fa7709cc09d3402af046620cbbe5c0`  
		Last Modified: Wed, 12 May 2021 20:07:13 GMT  
		Size: 5.7 MB (5714091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e7166d23985a06cbd08c0306a8b0ff5ef83c32e025fca0cb276ab170c27352`  
		Last Modified: Wed, 12 May 2021 20:07:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4068f3bcd403fb79c99aa76f07730960238098fe5808e2e7713b9faf6aaab3`  
		Last Modified: Wed, 12 May 2021 20:07:15 GMT  
		Size: 17.3 MB (17254278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c03a57df592a560d888220cba4e7fe2b06f5410505292cb0b1ad2a840a418f`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50169407a95b556efb846552a4c0bebf342bd6b93a2a9c515bfefa6f59a6f566`  
		Last Modified: Wed, 12 May 2021 20:07:10 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496cbceda3449349c3fad11bb07712b2eb6d339037f14cec194b00dcb559045`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f7ccad3e924ca06af935bb3f105e6ec1c7f5bf4dc794df7343b24e0f91c9b8`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd579cd39feec54d6644d366d86e5326892e849793b6b57c272cc6e005116a`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573df736fe3c12bfbf4e563cb2bdb7c0a7c36554e4b452b26e2629eb86117899`  
		Last Modified: Wed, 12 May 2021 20:07:07 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ca33eab3fdbb102f21d1e96d4d11a7456de6fd59991369612d137f075bb093`  
		Last Modified: Wed, 12 May 2021 20:07:08 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5801e9252319511ac618dd4ed87de597a11d991e9880cd9d10c3577f03298b`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3450f045350f8e214aeff68c08e2ded42fe0c6f2f85a179eda2727bbba21fd45`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceb8b0a02b9bdf3ee28de9083933a9b35766f20fd0151bf70062acdf1e86fc35`  
		Last Modified: Wed, 12 May 2021 20:07:05 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a47d134b87c7f8c844d59735119823a17b27f1f78afda8f29751f8d88671d7`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf10a836e3d3030e65f9608b9a8d425cc4dd5e8882fcdcc21084edb8bf7a3f8`  
		Last Modified: Wed, 12 May 2021 20:07:04 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9bfbeff13e0d1ffcc8229e74b5e564e3b5eeb7a947084db856f2fdc6e105cd`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdb78cf7ed64ccf3a6d810a56dad7b0035f86ae42749b6cb3ab6739fa8142617`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f443a34b54dbc5419852d048ce2da89de2fa90a64c375bfb1d784d9613a9247b`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bddd1bba1ef33f62ad9a2112d9781acc3e6af560bd67d42f67d31e28dd17b71`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 278.7 KB (278682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c02d5422753f120a445ecf958996865f559ba862d0b43666b212c10005e4ada`  
		Last Modified: Wed, 12 May 2021 20:07:02 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
