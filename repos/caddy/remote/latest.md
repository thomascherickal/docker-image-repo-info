## `caddy:latest`

```console
$ docker pull caddy@sha256:2c70c6bc2c9e2af8d3c7e1c33caccb3fdc7a2bebbab713e1921e1c98894ec7fc
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
$ docker pull caddy@sha256:c3b2e52162bebaf3b0d128780b3bffc4aa9ccb6953953892dd9d31495e15dc55
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.6 MB (14568035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b59636b1388443a36d8173a6ad50dbcf59de4b7786b8178ad9eb656ad6e9a387`
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
# Mon, 24 May 2021 18:23:10 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:23:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:23:13 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:23:13 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:23:14 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:23:14 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:23:14 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:23:15 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:23:16 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 80
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 443
# Mon, 24 May 2021 18:23:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:23:16 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:23:17 GMT
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
	-	`sha256:cba0aa26d56032b74c8c88c24edc5a2f7987ea418aaa0966f93ab53c62802c2f`  
		Last Modified: Mon, 24 May 2021 18:23:47 GMT  
		Size: 11.4 MB (11449656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712687f6a8ba00b8b6cb95bad7426eb9964fff3de9f5a7f66dedf6310e8a8c01`  
		Last Modified: Mon, 24 May 2021 18:23:45 GMT  
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
$ docker pull caddy@sha256:b767e2ec43a11bb1a211e3d7bc76c81d4a256f90084d5747367af6a9730e4f94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.1 MB (13121818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f930dc44ddd7a57e1d48aaeed66a69653dc4d5c15bdae6c378273cb55287f07b`
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
# Mon, 24 May 2021 18:19:32 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:20:01 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 18:20:18 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 18:20:25 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 18:20:32 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 18:20:39 GMT
VOLUME [/config]
# Mon, 24 May 2021 18:20:45 GMT
VOLUME [/data]
# Mon, 24 May 2021 18:20:51 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:20:59 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:21:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:21:15 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:21:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:21:34 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:21:42 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:21:51 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:22:03 GMT
EXPOSE 80
# Mon, 24 May 2021 18:22:10 GMT
EXPOSE 443
# Mon, 24 May 2021 18:22:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:22:21 GMT
WORKDIR /srv
# Mon, 24 May 2021 18:22:28 GMT
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
	-	`sha256:30c6214f82b33045060ad6f882d1ed7a5779be7a0883c4da8306ab03e9e2623c`  
		Last Modified: Mon, 24 May 2021 18:23:37 GMT  
		Size: 10.0 MB (10000116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52a67b9935763896cc7c3386cd93b5f7fbc80093549e39f460dc7e170f679f4`  
		Last Modified: Mon, 24 May 2021 18:23:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:40e8d6bc1ad5c4c4f902426841f39a594dd3842c212bed7ecbb66f312b5a4f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.9 MB (13938687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c9fccd235488bb04e0075ea4a47a8c102dce45c98cbba05e4d7d0d0ebb13b1e`
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
# Mon, 24 May 2021 17:41:40 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 17:41:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='dd5b347105df354edca8a77679bdf63e848de39cebcb8c1be3c2a38db16d1e8aee0e4ee84c1164333d15fa62b4491e4190f74efdff3d4f043a38d5e0c0eb3663' ;; 		armhf)   binArch='armv6'; checksum='5d21cdbf7875c9fe37dfd5a0480b94ce03c815e49fc9c2a8abebda5b4af47ebd58a60e5b9b95fd520a13d4da36d9cd74b9a5cb5dbdaf763366d594f731c46c00' ;; 		armv7)   binArch='armv7'; checksum='3a6a4441685e17be4b067b627d15892ef380dbfb23184b6b413468f78f1d7aae7ca540d35029490aadbad75ea9573cbb58ac7081bd518c1cbe9791dccdf92cd3' ;; 		aarch64) binArch='arm64'; checksum='b9946f6e105fe800394e371ad32212f1a6cc78b5cd187b1a146226f3635c245a924819cc66c36c84b6ffe230d339d1b3ede9bb0a71f94134f580a6dd01df411f' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='635888995efed987ebd2ebfa44e1bbba0f9901c2ce9897c5f97b769ba063339a1cc4055157c5ddc79121b8c79dabb6d6067b6df3ccaa49a3c4bd4f957bc3ac5b' ;; 		s390x)   binArch='s390x'; checksum='aa78736d3c600b34ccba4e2ef69475d62992282e2003a5586cbf9b66a1e16624cf48d2dab005dca5591cb2c6ffc2a39e3c847ea332f0f679b68d6d00520e143b' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 24 May 2021 17:41:47 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 24 May 2021 17:41:48 GMT
ENV XDG_DATA_HOME=/data
# Mon, 24 May 2021 17:41:49 GMT
VOLUME [/config]
# Mon, 24 May 2021 17:41:50 GMT
VOLUME [/data]
# Mon, 24 May 2021 17:41:50 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 17:41:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 17:41:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 17:41:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 17:41:54 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 17:41:55 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 17:41:55 GMT
EXPOSE 80
# Mon, 24 May 2021 17:41:56 GMT
EXPOSE 443
# Mon, 24 May 2021 17:41:57 GMT
EXPOSE 2019
# Mon, 24 May 2021 17:41:57 GMT
WORKDIR /srv
# Mon, 24 May 2021 17:41:58 GMT
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
	-	`sha256:f03e81629e078650b941a4beb267a6755133e90fa22a688bffb5df188e069c55`  
		Last Modified: Mon, 24 May 2021 17:42:37 GMT  
		Size: 11.0 MB (11029189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bbee1e7ec347a65e5e78b46b8fe541241e3f6c13a468785945abd0aaba24545`  
		Last Modified: Mon, 24 May 2021 17:42:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.1935; amd64

```console
$ docker pull caddy@sha256:1d0e1085c4e0fd3af411a60364e53d9e9ded463184467a4f1595116eb2e4c675
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2491869666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4dac2e4738ade97d420148e609ac6c7a6db9edb6db52f3a634814cbe64df1d0b`
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
# Mon, 24 May 2021 18:14:49 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:15:23 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:15:24 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:15:25 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:15:27 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:15:28 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:15:29 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:15:30 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:15:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:15:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:15:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:15:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:15:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:15:38 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:15:39 GMT
EXPOSE 80
# Mon, 24 May 2021 18:15:40 GMT
EXPOSE 443
# Mon, 24 May 2021 18:15:41 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:16:00 GMT
RUN caddy version
# Mon, 24 May 2021 18:16:01 GMT
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
	-	`sha256:d81697a0f2a55f882f55ccac9401c3dd272607c42f460a8549f30a1ebb26e0c8`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6400e9488fa4d970dad72e844be39d2d75b7d2c31501c6d6b23d6a1bc524f7c1`  
		Last Modified: Mon, 24 May 2021 18:22:57 GMT  
		Size: 11.9 MB (11930419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c5b5da05058a691610222ba26189e6f6c28b9ede612bec34b4ed5dea3691b92`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:197bdfed68cccee24a939b4dd69fea66e2dc7827a4017bf444bdd2c90e959f6a`  
		Last Modified: Mon, 24 May 2021 18:22:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:474f7ecfe9858ec31d5203cc051d4063e0ad4acd2af33e4568f49d9e4b75e41b`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026dffad92f6dace75c209e6f261b00cf847128dd907ffa4ac9f944e9ae054e`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c534d757d31dc1e6130a58f06b95d25d61f32e015e329cd2227a1bed890280`  
		Last Modified: Mon, 24 May 2021 18:22:52 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31071464c175eef4ea5843313a962e550e530c0a4c12fd997c6ace04fed5d0e0`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3035f85e6f0ef498e48d22a196b3dca2d1feff90554b2f1fbbd3062a92ffccd2`  
		Last Modified: Mon, 24 May 2021 18:22:51 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caffd6e1f83b89b2831eab80faf22c370ad73519467e80354cb56ee96eed7fe3`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285714c5a6fb40773b7e624641f8e036180ab3424ee89b84f3fbbd79d7108eec`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872e853821b7661d1e753ef89a95c2525171915b5dec31950f7b05f4492eb40c`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7958b6b43cba2b3e1a20dc772e84541237901c32ec6dba998eb300627b2e343`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8089fe8b99a3884b64fb515b432248ed2433347b16efe53190c08624ec8bcf8f`  
		Last Modified: Mon, 24 May 2021 18:22:49 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e25c6bfe294987f6c4c3a677078ea11dd90d54892fff638abed3d5a8602360c`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1757220b38637dda7da307ac64a4eefb9226cd9e13d613ab9bb839997c0c2aa8`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a748ef821631911b8abd470af8b29305283a82e1b5da1d2459257d8308576a2`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afa22970d4f705eac4e8ea2ac4a7f3e89cfc01035b6ff0bf8998c146fe4d9a96`  
		Last Modified: Mon, 24 May 2021 18:22:47 GMT  
		Size: 317.9 KB (317938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2477d94c5c1388771379c903fc8931c2531d21a7ccbef4b3b7e2d6461fb19fdd`  
		Last Modified: Mon, 24 May 2021 18:22:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.14393.4402; amd64

```console
$ docker pull caddy@sha256:d530e436d6d892bc2662481a943d230921dd8d5b2a26de0d99c32abb59ce1973
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5819027610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:189fbf35362e472481d308f9fbecfeda8962471fccd521c1cdd2165bfff22c08`
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
# Mon, 24 May 2021 18:16:16 GMT
ENV CADDY_VERSION=v2.4.1
# Mon, 24 May 2021 18:17:59 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Mon, 24 May 2021 18:18:01 GMT
ENV XDG_CONFIG_HOME=c:/config
# Mon, 24 May 2021 18:18:02 GMT
ENV XDG_DATA_HOME=c:/data
# Mon, 24 May 2021 18:18:03 GMT
VOLUME [c:/config]
# Mon, 24 May 2021 18:18:04 GMT
VOLUME [c:/data]
# Mon, 24 May 2021 18:18:05 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Mon, 24 May 2021 18:18:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 24 May 2021 18:18:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 24 May 2021 18:18:09 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 24 May 2021 18:18:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 24 May 2021 18:18:11 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 24 May 2021 18:18:12 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 24 May 2021 18:18:13 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 24 May 2021 18:18:14 GMT
EXPOSE 80
# Mon, 24 May 2021 18:18:15 GMT
EXPOSE 443
# Mon, 24 May 2021 18:18:16 GMT
EXPOSE 2019
# Mon, 24 May 2021 18:19:09 GMT
RUN caddy version
# Mon, 24 May 2021 18:19:10 GMT
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
	-	`sha256:eba52519d045fbbd4b405dea0a101b9ede50767ce1b8b92f0b0a9708dc3a3492`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073bc62336c22adb06e7c530733538c823c0e30b591f536ca853dd86ff16e632`  
		Last Modified: Mon, 24 May 2021 18:23:26 GMT  
		Size: 17.2 MB (17244195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319fcbb76d6ed2f5920ae3cf875486281ed4d5edc53c630c8c6ad581efc92594`  
		Last Modified: Mon, 24 May 2021 18:23:22 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d372740cbc98799ef99cd14fe521f6c8bc0202f7e6eb418f8db3e6cae94caf60`  
		Last Modified: Mon, 24 May 2021 18:23:21 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0c1957ce089769a88ac826364c0cb191ae826407602ccf505c76ee34afa10c8`  
		Last Modified: Mon, 24 May 2021 18:23:20 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e022ba7739dc4609e4838ae24c6930ccdc82d0721cc978c71a7e036122adf228`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5716dc07e962e5602a2cecf1a5b63c75352ad0e48b06b30070ad5cd4a31993`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadc94100cd9e1fb3620069275788a9e1b912502dcd7966b4d624ecba5f88690`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7790197c85ec7196ed9b956d8f481e8f382479a3b8e20db4d8e564f14331eb42`  
		Last Modified: Mon, 24 May 2021 18:23:19 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60939c5f58f38df81a8563072d42fcd4fb79292dbf5ce4d31a46f840e777fb88`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d5876f07c48377c92817efa2b077cfe4c05822b08a1916d350b5e8ee682b50`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2933951452131d66acb34683269ade093ebb9faf312436b0a601168cb6e2fe68`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ad33c6332b1b2a8e806339fd2978dd9a8919fc98d48fc0ae6a58ad07870cec`  
		Last Modified: Mon, 24 May 2021 18:23:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b44c787b930665927a13e544b5d3d7243caae27d4d9a6f9502f985e8483af61`  
		Last Modified: Mon, 24 May 2021 18:23:16 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e86dd1b42134f467b929f29aa052bdca8a20ccbb6ff1332575ef7843b962243`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3288b716f0b64cb14a9da486b126557c121b9a71476d5aea6a1be399a82bb14b`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83f9226706657b746cb502303856ebeca1a6cda85b1aea65196506c3e3faa4a`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fc7b2fb07d7a4265b695bf44d6d3378e7f0202a6c8fd0d359f766886070802`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 266.6 KB (266650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5cde5c4ac8767e62fceac7aed63a74d7935277b8087425319abfe8e22f7bb37`  
		Last Modified: Mon, 24 May 2021 18:23:14 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
