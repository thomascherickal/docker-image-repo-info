<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `caddy`

-	[`caddy:2`](#caddy2)
-	[`caddy:2-alpine`](#caddy2-alpine)
-	[`caddy:2-builder`](#caddy2-builder)
-	[`caddy:2-builder-alpine`](#caddy2-builder-alpine)
-	[`caddy:2-builder-windowsservercore-1809`](#caddy2-builder-windowsservercore-1809)
-	[`caddy:2-builder-windowsservercore-ltsc2022`](#caddy2-builder-windowsservercore-ltsc2022)
-	[`caddy:2-windowsservercore`](#caddy2-windowsservercore)
-	[`caddy:2-windowsservercore-1809`](#caddy2-windowsservercore-1809)
-	[`caddy:2-windowsservercore-ltsc2022`](#caddy2-windowsservercore-ltsc2022)
-	[`caddy:2.6`](#caddy26)
-	[`caddy:2.6-alpine`](#caddy26-alpine)
-	[`caddy:2.6-builder`](#caddy26-builder)
-	[`caddy:2.6-builder-alpine`](#caddy26-builder-alpine)
-	[`caddy:2.6-builder-windowsservercore-1809`](#caddy26-builder-windowsservercore-1809)
-	[`caddy:2.6-builder-windowsservercore-ltsc2022`](#caddy26-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6-windowsservercore`](#caddy26-windowsservercore)
-	[`caddy:2.6-windowsservercore-1809`](#caddy26-windowsservercore-1809)
-	[`caddy:2.6-windowsservercore-ltsc2022`](#caddy26-windowsservercore-ltsc2022)
-	[`caddy:2.6.4`](#caddy264)
-	[`caddy:2.6.4-alpine`](#caddy264-alpine)
-	[`caddy:2.6.4-builder`](#caddy264-builder)
-	[`caddy:2.6.4-builder-alpine`](#caddy264-builder-alpine)
-	[`caddy:2.6.4-builder-windowsservercore-1809`](#caddy264-builder-windowsservercore-1809)
-	[`caddy:2.6.4-builder-windowsservercore-ltsc2022`](#caddy264-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.4-windowsservercore`](#caddy264-windowsservercore)
-	[`caddy:2.6.4-windowsservercore-1809`](#caddy264-windowsservercore-1809)
-	[`caddy:2.6.4-windowsservercore-ltsc2022`](#caddy264-windowsservercore-ltsc2022)
-	[`caddy:alpine`](#caddyalpine)
-	[`caddy:builder`](#caddybuilder)
-	[`caddy:builder-alpine`](#caddybuilder-alpine)
-	[`caddy:builder-windowsservercore-1809`](#caddybuilder-windowsservercore-1809)
-	[`caddy:builder-windowsservercore-ltsc2022`](#caddybuilder-windowsservercore-ltsc2022)
-	[`caddy:latest`](#caddylatest)
-	[`caddy:windowsservercore`](#caddywindowsservercore)
-	[`caddy:windowsservercore-1809`](#caddywindowsservercore-1809)
-	[`caddy:windowsservercore-ltsc2022`](#caddywindowsservercore-ltsc2022)

## `caddy:2`

```console
$ docker pull caddy@sha256:cb9a70e2fe64b1f0a871628e2fa71efcfb3f632dacc0a210ca8d484445cca70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:eefd3d61e9ee8f35e046f614982d9a970006e3943c6e5f09957a4048f4c80d35
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
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:e849a3ca3945f7122242440191cec8d4d568ac2f42add780ac7b4d22b5356c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:c33a779d8fe816ecce63c84891fef7ec2eb410397a53d43428f086ac19cf949f
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
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6096f01ef551f4b7b079e437bc16af11067298c7b1618582203d017fc7781c27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bab627d047890c81cb42f4f8e25a90a9217b48488a3c15980d0501244b7d5544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:3f6d61ed02f8e689b02604b64416863fc5f161fe638e8facb43ed78e89849065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dd8b35b944648b6de74e54e981624f78ee1745fa84d8c7a02bce54878668e019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:85e9a8d2824c1d06afd808a980707fa129a3a734da68abfcbcb91733acdd0d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:cb9a70e2fe64b1f0a871628e2fa71efcfb3f632dacc0a210ca8d484445cca70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:eefd3d61e9ee8f35e046f614982d9a970006e3943c6e5f09957a4048f4c80d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder`

```console
$ docker pull caddy@sha256:e849a3ca3945f7122242440191cec8d4d568ac2f42add780ac7b4d22b5356c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:c33a779d8fe816ecce63c84891fef7ec2eb410397a53d43428f086ac19cf949f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6096f01ef551f4b7b079e437bc16af11067298c7b1618582203d017fc7781c27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bab627d047890c81cb42f4f8e25a90a9217b48488a3c15980d0501244b7d5544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:3f6d61ed02f8e689b02604b64416863fc5f161fe638e8facb43ed78e89849065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dd8b35b944648b6de74e54e981624f78ee1745fa84d8c7a02bce54878668e019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:85e9a8d2824c1d06afd808a980707fa129a3a734da68abfcbcb91733acdd0d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4`

```console
$ docker pull caddy@sha256:cb9a70e2fe64b1f0a871628e2fa71efcfb3f632dacc0a210ca8d484445cca70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6.4` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-alpine`

```console
$ docker pull caddy@sha256:eefd3d61e9ee8f35e046f614982d9a970006e3943c6e5f09957a4048f4c80d35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.4-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder`

```console
$ docker pull caddy@sha256:e849a3ca3945f7122242440191cec8d4d568ac2f42add780ac7b4d22b5356c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-alpine`

```console
$ docker pull caddy@sha256:c33a779d8fe816ecce63c84891fef7ec2eb410397a53d43428f086ac19cf949f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.6.4-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6096f01ef551f4b7b079e437bc16af11067298c7b1618582203d017fc7781c27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2.6.4-builder-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bab627d047890c81cb42f4f8e25a90a9217b48488a3c15980d0501244b7d5544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore`

```console
$ docker pull caddy@sha256:3f6d61ed02f8e689b02604b64416863fc5f161fe638e8facb43ed78e89849065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6.4-windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-windowsservercore` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:dd8b35b944648b6de74e54e981624f78ee1745fa84d8c7a02bce54878668e019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:2.6.4-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:85e9a8d2824c1d06afd808a980707fa129a3a734da68abfcbcb91733acdd0d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:2.6.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:eefd3d61e9ee8f35e046f614982d9a970006e3943c6e5f09957a4048f4c80d35
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
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:e849a3ca3945f7122242440191cec8d4d568ac2f42add780ac7b4d22b5356c88
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:c33a779d8fe816ecce63c84891fef7ec2eb410397a53d43428f086ac19cf949f
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
$ docker pull caddy@sha256:a6ac9d3116a00f231d79ec6e0289829484ff93f061f563e3e8bcf8fd47b8838e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131462251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f925b0539e9a9855288b9875d063ca9bf618c151b6b259d4bfd84a7b14e8f3eb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 20:34:05 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 20:34:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:54 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:30:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:29 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:29 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:30 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:20 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:20 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:20 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:22 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:22 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:22 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85791d961cd3578144eb3d64a9716fa35c198c4ae9202b07eb0f2de9127a7907`  
		Last Modified: Wed, 29 Mar 2023 20:41:12 GMT  
		Size: 284.8 KB (284812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39647feab07db90c27088e25bf6657b494826426f0647bf9366b6aef1b8f1eb1`  
		Last Modified: Tue, 04 Apr 2023 18:35:26 GMT  
		Size: 122.4 MB (122385644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4375bc5d93b8cea280f2b2c978d22b7a7e69390b483c2d643a4f98303576e69d`  
		Last Modified: Tue, 04 Apr 2023 18:35:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ba3905ec9081a3d811719d8b736830bc138e457d8e0f8db168e439cad20f96`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 4.2 MB (4198839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db536c6f7a3ee071e4847c9a3d61e18f0758af093585ba7f28009c8fe12a093f`  
		Last Modified: Tue, 04 Apr 2023 18:51:36 GMT  
		Size: 1.2 MB (1217833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119ea5cbe0d910e44ce6f510f6e3f1e5d81430dd683c81c64bd2672dfb68e9fc`  
		Last Modified: Tue, 04 Apr 2023 18:51:35 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:6437946c03ab9365cde9efb2d571f0108285fc367290e98747cf916b7dceaa04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127474264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d676ab02f07c9dc12522a9bcdbd48d3b684ef89046fe1439c35559f08bdb68c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:09 GMT
ADD file:2dd294d20c0b500c8fed6b410b059429b36f51cd48a45eaf7a06ecbef9e2a3bb in / 
# Wed, 29 Mar 2023 18:01:09 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:11:18 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 19:11:18 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:34:30 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:36:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:36:20 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:36:20 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:36:20 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:36:21 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:02:53 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:02:53 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:02:53 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:02:55 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:02:55 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:02:55 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:75257e753735e4ff78fae2d44018022a6ac775290e02103713a70699ece7576e`  
		Last Modified: Wed, 29 Mar 2023 18:01:52 GMT  
		Size: 3.1 MB (3110802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeff4fbf60178fec9f066beaffd29f01058a664c1a12ff62dbf90800266066a9`  
		Last Modified: Wed, 29 Mar 2023 19:20:39 GMT  
		Size: 286.2 KB (286215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:637df33b94b1d1127a4f4dd6449ed4b0a2f72ee8479f67f33cbf17728ccb733e`  
		Last Modified: Tue, 04 Apr 2023 18:47:04 GMT  
		Size: 118.7 MB (118749945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638cdf73ee309245708bdf59d03827b61b643f289953d21613314b3eeb63b2ac`  
		Last Modified: Tue, 04 Apr 2023 18:46:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de0147f684ee2e7f73d5466a0efd83770f009d53cf4d1f59870f27c8e103421`  
		Last Modified: Tue, 04 Apr 2023 19:06:00 GMT  
		Size: 4.2 MB (4160675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8791bb2f9dbd430ff0638f74c5b73d90ae6ae980e4909df01d2ff8957c88623f`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 1.2 MB (1166067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3128c603a26daa252d6721eddac3059a23d1d52d57a86ba064f66d8aeca6a086`  
		Last Modified: Tue, 04 Apr 2023 19:05:59 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:a825f4dc9334d8d6c2f121ab062acddb50bbfb46d8b12ecb47b02f98263c149e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126555891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c8ed5991bf75bc0ba20443cb0b846109ac7a9084c44272665db3f448853c144`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:03:38 GMT
ADD file:959fa0ffb60c37c4fdc0d32ac31511f8dead32ef7f4bd848b11ff144a6b37012 in / 
# Wed, 29 Mar 2023 18:03:38 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 01:14:25 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 01:14:25 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:39:07 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:40:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:40:53 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:40:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:40:53 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:40:53 GMT
WORKDIR /go
# Tue, 04 Apr 2023 19:18:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 19:18:17 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 19:18:17 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 19:18:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 19:18:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 19:18:19 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:fd4b2aeb476b6c2c0c3049dae919de20fe09e90deac95e3181d717055cbe6707`  
		Last Modified: Wed, 29 Mar 2023 18:06:56 GMT  
		Size: 2.9 MB (2868519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c307ec99e547bddce4091b501a5d22ea790937f2dfe9d02cba52960d9b78fbe`  
		Last Modified: Thu, 30 Mar 2023 01:28:08 GMT  
		Size: 285.4 KB (285438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feebe34dac5c9ca7e397b6cecf24ba4e82590afbb261f9409cbb0faf51925d1b`  
		Last Modified: Tue, 04 Apr 2023 18:51:45 GMT  
		Size: 118.5 MB (118508772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13c84ba94d34586ade88068b526e83264132815b36d6c962ebad1982b22894`  
		Last Modified: Tue, 04 Apr 2023 18:51:27 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3f6d4dcf990fe2003bd42d43b9ec7b8873f6f301b902e0ca6ddcbab3622491`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 3.7 MB (3729273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4cbb25f5821c55b96b86ce9f9f18697267716ecd63515847ff4244acb2f8d61`  
		Last Modified: Tue, 04 Apr 2023 19:18:32 GMT  
		Size: 1.2 MB (1163329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be5a1f3a413a1c2a33bbadbf06b541f10b2c83088f5a617659525d852231d45`  
		Last Modified: Tue, 04 Apr 2023 19:18:31 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:8f6ab9037936481f14bf04d24373c70e7121d4d47e5ca9384fcaa0eb32400fef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125865485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f09028c04a63d67925b32c0176cc821c365d2d6f4902894ee830247d63897273`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:58:47 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 03:58:47 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:28:46 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:29:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:30:00 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:30:00 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:30:00 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:30:01 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:50:03 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:50:03 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:50:03 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:50:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:50:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:50:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed15518f570754b8336aff46024845ecb67da1ab7729e4d5701a42fa4c19396b`  
		Last Modified: Thu, 30 Mar 2023 04:04:23 GMT  
		Size: 286.3 KB (286258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18aa78607fb3d45a76cd37d28ee56a0083f8138de2124b2fb3cb4a2144619607`  
		Last Modified: Tue, 04 Apr 2023 18:34:16 GMT  
		Size: 116.9 MB (116949710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f7a98b2bad79513332aaacf90f17ff3ac685b3dd33dfb8dfe82e03762347`  
		Last Modified: Tue, 04 Apr 2023 18:34:04 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a64e664c739afb7b2f5c3f7dbac02491b794497a844e22f573f6257bf75d33`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 4.2 MB (4243367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f1b0eebd4cc4d89b0a7e836aa6b57248555ac6d0c3267a02dd730c403cf3d0`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e63be9eb53815bbd0165abd9f6dd09b1cb2a5c3d0142ee59df98a0ef5f817f4`  
		Last Modified: Tue, 04 Apr 2023 18:50:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:5db53505e52855f79c086219dd7ef08a34fbf94209f70055e6b1e56e87074312
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126598190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65255156fbe253062b8ed1429ec52de7a0e96ae12fa548653a8ac29c9467d07c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 05:16:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 30 Mar 2023 05:16:54 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:32:27 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:35:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:35:28 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:35:28 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:35:30 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:35:31 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:58:14 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:58:14 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:58:14 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:58:15 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:58:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:58:17 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:58:17 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5d0873c74e9df3bedfdfb2fb4562e46fe6d0981207b57a0f358299331b74fb`  
		Last Modified: Thu, 30 Mar 2023 05:28:38 GMT  
		Size: 286.7 KB (286660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d5545da41d548e72e043241d1cab3ed6ba29d7c52aef74220c4c630d44701d5`  
		Last Modified: Tue, 04 Apr 2023 18:42:00 GMT  
		Size: 117.3 MB (117325966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda5d8fdb7bf5b638b0ae5f09a077654d48a6d206a8d0935063bff08c1d4ebd`  
		Last Modified: Tue, 04 Apr 2023 18:41:34 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2fd33a498d8bb630318591984483b19b7632f0499cbad2104aefe7f4c9d2e1`  
		Last Modified: Tue, 04 Apr 2023 18:58:34 GMT  
		Size: 4.5 MB (4488178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b161d9a32bed5317b7d1a7a9ca0ad64e76946ce9aef9be3a226f2e8b4d26ff10`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 1.1 MB (1105890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:126c9267798ec24f1d01d69b6f6bf7b2fb29e2654065edb1de74db6738cba1f1`  
		Last Modified: Tue, 04 Apr 2023 18:58:33 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:77bf4c28655d7a62ea08548a6df76fb15124e6de96e2f69bc6fce1e2f747d107
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129617824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f71dba195e160c90525f20e437fefd0b9adb350a61f4c8bb4c12d512c606dd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:57:20 GMT
RUN apk add --no-cache ca-certificates
# Wed, 29 Mar 2023 22:57:20 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:29:11 GMT
ENV GOLANG_VERSION=1.19.8
# Tue, 04 Apr 2023 18:31:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.8.src.tar.gz'; 		sha256='1d7a67929dccafeaf8a29e55985bc2b789e0499cb1a17100039f084e3238da2f'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 04 Apr 2023 18:31:11 GMT
ENV GOPATH=/go
# Tue, 04 Apr 2023 18:31:11 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 04 Apr 2023 18:31:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Tue, 04 Apr 2023 18:31:12 GMT
WORKDIR /go
# Tue, 04 Apr 2023 18:51:30 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 04 Apr 2023 18:51:30 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 04 Apr 2023 18:51:30 GMT
ENV XCADDY_SETCAP=1
# Tue, 04 Apr 2023 18:51:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 04 Apr 2023 18:51:31 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 04 Apr 2023 18:51:31 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a43eca718641eeaefd2ef545022e8742fa976dc3428d4ebb9fbfb3736cb1ca`  
		Last Modified: Wed, 29 Mar 2023 23:06:29 GMT  
		Size: 285.0 KB (285037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10697997d381ca1620b9c3d9feba3aca3647fe5d9818d7f57df8827e1b49035e`  
		Last Modified: Tue, 04 Apr 2023 18:35:33 GMT  
		Size: 120.8 MB (120814883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce91e737e0f005857cecd26d6b368de29fd6f89757612e6a2a882518a3fe6384`  
		Last Modified: Tue, 04 Apr 2023 18:35:17 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab459779238b4501357166b0639745378d763ea0b957aad51e4fe807f4d7038`  
		Last Modified: Tue, 04 Apr 2023 18:51:50 GMT  
		Size: 4.2 MB (4171754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7d316158a7768a7292c6ed4c4bb4ff725a6fb06d66446603fc198fe6b50f89`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 1.2 MB (1170406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:888f019d3f6df4530a27f80fde7576a46b1b165f30810861dcd970562b965e98`  
		Last Modified: Tue, 04 Apr 2023 18:51:49 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:6096f01ef551f4b7b079e437bc16af11067298c7b1618582203d017fc7781c27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:f25f53de4ebf9a09c5dbd15bb1c89058e05e317e3e0c1b85bc3d3a9e6ea7db63
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2256673861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4790ca87985aee382fbf1c940bcccd5825ef2b289fbe772ab081684e223e1ce`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:54:13 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:54:14 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:54:15 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:54:16 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:56:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:56:40 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:57:53 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:15:47 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:22:24 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:22:27 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:07:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:07:25 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:07:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:07:27 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:09:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:09:39 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a6de00b28bac0666d00c5a680ca62116074e664878553846026da5c3116e14`  
		Last Modified: Wed, 12 Apr 2023 02:32:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aefb03e237e07e11ef0bcedf393cddb3fea112dbf95771c2a8fd09138f5fa331`  
		Last Modified: Wed, 12 Apr 2023 02:32:49 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ef0a611281437670a551a9d388018ca6583c5f934b5f26514f7cdd8d1a8771`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e751ae5812845616a66f9446726d4aba077b086487190ab0cf05ddd245b9c8`  
		Last Modified: Wed, 12 Apr 2023 02:32:48 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d802cb7e5f3a9b618e9765e831db7ae04a9097f456a4cf70b15706bbb289a5`  
		Last Modified: Wed, 12 Apr 2023 02:32:55 GMT  
		Size: 25.6 MB (25604110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30278f60b48b729152d141e9b3a5e94c8ed1d95059849d727e1dafd7331f1bbc`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0812ea54b5317c55bbbec51b566520e84db2b58e2b8d86f92fd75ab23d0694`  
		Last Modified: Wed, 12 Apr 2023 02:32:46 GMT  
		Size: 332.4 KB (332356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd4656f51c41856eeec44891f68027991b45e943a65ddc723f5368b95803957d`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bff19f0ed42678ffce803e906f1522ae37e24c2ea6af0c7131189c72a47913`  
		Last Modified: Wed, 12 Apr 2023 02:37:12 GMT  
		Size: 157.8 MB (157795199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083b6ab53364edfffb935c1eb86e032fc10f2d6ca49f8bbfd8403d9272c874cf`  
		Last Modified: Wed, 12 Apr 2023 02:36:23 GMT  
		Size: 1.6 KB (1558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc05b2a96bef95980b24b4b35ca805a81c4fc286cdba8b4172c3a602536989`  
		Last Modified: Wed, 12 Apr 2023 03:13:17 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc6fb2f2a659374956800335d0f0146c92114ce290041d1c05f5ba8ed11f5fa`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5595bd45cbdea75e128c169d10e8ce32d143314bd3977911dec30edd258ab8b8`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b08adc6114bfae4b48fcb3199fc40634476d68bb97bd9bdeca335f6736d9ac83`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05541672e96f3bc5c39448cca01fc04474603eb399815d815a2e587019363b0a`  
		Last Modified: Wed, 12 Apr 2023 03:13:16 GMT  
		Size: 1.6 MB (1632522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a6591cd2895825dc9a45683e9c9590ffdc4836b71f54f1ff4cad423745df26`  
		Last Modified: Wed, 12 Apr 2023 03:13:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:bab627d047890c81cb42f4f8e25a90a9217b48488a3c15980d0501244b7d5544
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:df50214b07a9dc73b18c311995a11aba883abb04f886cd0d03f21b727f58a0e9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1948856230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ab8eca451e97dd9533117642b8d4f4115096292a26ae4463f655b90ddc45da6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 01:49:43 GMT
ENV GIT_VERSION=2.23.0
# Wed, 12 Apr 2023 01:49:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 12 Apr 2023 01:49:45 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 12 Apr 2023 01:49:46 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 12 Apr 2023 01:50:32 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 01:50:33 GMT
ENV GOPATH=C:\go
# Wed, 12 Apr 2023 01:51:03 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 12 Apr 2023 02:11:16 GMT
ENV GOLANG_VERSION=1.19.8
# Wed, 12 Apr 2023 02:15:38 GMT
RUN $url = 'https://dl.google.com/go/go1.19.8.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '433558e81b8be2983f370bf8e21ac52e76e9e1e50c69b6dc0047f1b6acde97fd'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 12 Apr 2023 02:15:39 GMT
WORKDIR C:\go
# Wed, 12 Apr 2023 03:09:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:09:57 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 12 Apr 2023 03:09:58 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:09:59 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 12 Apr 2023 03:11:25 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 12 Apr 2023 03:11:27 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb4eb152e8775777886c34769c9441311dc4cfa18739a77add3a28f4146876c0`  
		Last Modified: Wed, 12 Apr 2023 02:32:01 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b178567290fd84aae46273380c8bbab148ca30148807f2152ab814a3404cf485`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd32032c86ce46fc3bd16fd2626e5ef1ad026803eb85788f8cd91806b9b8d54`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c72e3d7691a1228d8cb57c6aee1dfb1257d1f0a9ac87e1f46a51b80ca7496b1`  
		Last Modified: Wed, 12 Apr 2023 02:31:58 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07645ae8480c674321c57e55fce61bb16b6c09f94b07982e8ae4730746807e61`  
		Last Modified: Wed, 12 Apr 2023 02:32:06 GMT  
		Size: 25.9 MB (25855167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7114ddfb58c5199edc3cc1e070d9c70422f31bb08a24e9a22a810a95267f5dc4`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f2024bc0d3314bfc3e125a3386eb0b2fda1ac02c72426efde256013cf401972`  
		Last Modified: Wed, 12 Apr 2023 02:31:56 GMT  
		Size: 544.5 KB (544547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdae693610d92eb8ccd68d4abee8b1dcbeae17c1f6240fb7a1b21eb5b42f795e`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe6fd19fd6ef915467bef8fd042cd7ec1c81bd5adf5f09b26466e4b254034b0`  
		Last Modified: Wed, 12 Apr 2023 02:36:14 GMT  
		Size: 158.0 MB (157986622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e35d513f3dac85b04747754cdafe72878ef3b4c4517f7e7e5938ffafac37f`  
		Last Modified: Wed, 12 Apr 2023 02:35:23 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c218317b53deb5a3a51db2b28c84802667a220220ac76e0665ba55064b1d378a`  
		Last Modified: Wed, 12 Apr 2023 03:13:41 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f91573e9407524377d8f3f1fb70285a197c9c1a16b519ccaac059b81123157`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3319a73f5ed203dce8de1cb1bada296a7dd4d3dbaa953c66e25f6ca1fc8c36c`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ca55f0e501bbaf464222954d0e88d553a95b2854c04b9a08cdd5f7a2fac343`  
		Last Modified: Wed, 12 Apr 2023 03:13:38 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a2b42ff04eb6bd0e85380378e7cd650cf6b1863ebcb320bb0b972d3f82460e1`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.8 MB (1849403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff3133fe5b68a4ff4a157733c0993c62895cfc692ece90378791a5839e0dcb0`  
		Last Modified: Wed, 12 Apr 2023 03:13:39 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:cb9a70e2fe64b1f0a871628e2fa71efcfb3f632dacc0a210ca8d484445cca70a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:5acae6b87b26a591d6d14ec2704b7f2cd94b888ad62af16a02356d3124198ede
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17449151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86ab4e60cac2e943fc115f5a9ec4f7b91ee165fbabc01b3f00963ce6319d1101`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:40:48 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 19:40:49 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 19:40:49 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 19:40:51 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 19:40:51 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 19:40:52 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 80
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 19:40:52 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 19:40:52 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 19:40:52 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f137c1fd65aa258552c9e586c735e093ab17bfd56f8b955a45368f75d9dd186`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 351.2 KB (351170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123731571dfc917eae08527f983c1f454a9fed97dd0454272dbd89c24e8a32c7`  
		Last Modified: Wed, 29 Mar 2023 19:41:06 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab4cbb8b7b7cfb79fecb20ac12ecf5d3d8cc9c9fe1d05c4dad071564f4748b6`  
		Last Modified: Wed, 29 Mar 2023 19:41:08 GMT  
		Size: 14.3 MB (14282622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:b27532c3b8bee89c27501e93b81d69b60f2bab459e9b967f39d2ccec151c93b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16582574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbe9d5fca028312523db46b46629b828c790b9f89b13f31b434725f6232a15c4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:01:11 GMT
ADD file:c5e68ad58a515830d33f20488adffa6af47be2e332543c747b8931cab7444e59 in / 
# Wed, 29 Mar 2023 18:01:11 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:46:53 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:46:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:46:54 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:46:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:46:56 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:46:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:46:57 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:46:58 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:46:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c4ddbcc13e08e4ef30f810d8afad41fd6994bd8af7d37746d0ea33d8813968fc`  
		Last Modified: Wed, 29 Mar 2023 18:02:04 GMT  
		Size: 2.6 MB (2616846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f04d50a24d37f7e9368a95cb9088fa7d5bf8cdfbe3929c8765c4f954507d2`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 345.9 KB (345890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5a70f8f2e1b052396c9849792ea86786d09a1ff21867462d2a06d4985f9d65`  
		Last Modified: Wed, 29 Mar 2023 18:53:24 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b1bd3eb25fd6c488f51f95377dc1d17fdcc2c687a3042c82d99a84c306137d`  
		Last Modified: Wed, 29 Mar 2023 18:53:26 GMT  
		Size: 13.6 MB (13612281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:4ad2390026191553fc198da4f8d3c9addb4d24b46d2f92e23195a022ba52a1d3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16365735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f58ffc22bc39150d1ac5af1b1b8490dc499fc410a2eef48a01d0c7c8cb2c978`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:04:21 GMT
ADD file:68992157dbe7c3a454c26656c7bcb497794c1008ead5e078b2928ce165cd65cd in / 
# Wed, 29 Mar 2023 18:04:21 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 00:39:33 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 00:39:34 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 00:39:34 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 00:39:36 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 00:39:37 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 00:39:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 80
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 00:39:37 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 00:39:38 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 00:39:38 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d378ffb313542b797defad9ec843de710c353f40e17e124e74f7e874971429ee`  
		Last Modified: Wed, 29 Mar 2023 18:07:08 GMT  
		Size: 2.4 MB (2420546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b21b970f1be3dd1f6ad93f4233bb05eebdbc1caebe8ab6c769093da8666c467`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 342.7 KB (342668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac71d5cd008392394c1e0bec73660595a0e8a2dbe6ab5083c202f2c8a32f06`  
		Last Modified: Thu, 30 Mar 2023 00:40:05 GMT  
		Size: 7.6 KB (7556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b7d87e28f1b54178ce40ce4129f58954d0716466859c7cef74b3db045ce73e`  
		Last Modified: Thu, 30 Mar 2023 00:40:07 GMT  
		Size: 13.6 MB (13594965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5c676a59917cfb48a9c8a8a60df8314bddbde15524450db55f25e2aa598850ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16130847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cac8e331cadbcef5644aae5d39704fc6ec4c5d6c734c2458509675805ca9b1f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:20 GMT
ADD file:a6a2f69b60d7d27bc6e2b9b7e9910dabdc3f5e3702c2345d26a7dc8c603ae595 in / 
# Wed, 29 Mar 2023 17:39:20 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:54:55 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 03:54:56 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 03:54:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 03:54:58 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 03:54:58 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 03:54:59 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 80
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 03:54:59 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 03:54:59 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 03:54:59 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:547446be3368f442c50ff95e2a2a9c85110b6b41bbb3c75b7e5ebb115f478b57`  
		Last Modified: Wed, 29 Mar 2023 17:39:56 GMT  
		Size: 2.7 MB (2709344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c0f047cc7662980b0739593b7d9ae110e54e817ec4cf6b890d854e1321705cc`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 350.2 KB (350158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0176485b11b9294cec973ec9fc20ff1a0caf1c601f31cdf81400b26bdc0236`  
		Last Modified: Thu, 30 Mar 2023 03:55:11 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e02e2e7f6d534004c3e59c7fbbe30bc0b90cdea9aa850214e9db3cfd927bf2a`  
		Last Modified: Thu, 30 Mar 2023 03:55:13 GMT  
		Size: 13.1 MB (13063787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:962bb98297c84cbd2004b63e0d4f8f728fb3282162b62031a2728af1d5c95d72
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a59a35c3b20b118606a348555696e80b6f71a180fe66b154f37be4495ef06245`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:34 GMT
ADD file:00a20a25a46ff8ebd9bc78b5b8c6fc5b1dc8ae73d5a42048fa5769a2b2e717c7 in / 
# Wed, 29 Mar 2023 18:16:34 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:39:08 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Thu, 30 Mar 2023 04:39:10 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Thu, 30 Mar 2023 04:39:11 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 04:39:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 30 Mar 2023 04:39:15 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 30 Mar 2023 04:39:16 GMT
ENV XDG_DATA_HOME=/data
# Thu, 30 Mar 2023 04:39:16 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 30 Mar 2023 04:39:17 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 30 Mar 2023 04:39:18 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 30 Mar 2023 04:39:19 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 80
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443
# Thu, 30 Mar 2023 04:39:20 GMT
EXPOSE 443/udp
# Thu, 30 Mar 2023 04:39:21 GMT
EXPOSE 2019
# Thu, 30 Mar 2023 04:39:21 GMT
WORKDIR /srv
# Thu, 30 Mar 2023 04:39:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:d80736dee7a63492583c90bab1ab07f987ed5e10dfb16fd3f025df3a2d65f1c6`  
		Last Modified: Wed, 29 Mar 2023 18:17:28 GMT  
		Size: 2.8 MB (2804670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29ab2c4253c7f672d14502ad6ef639d71074661b50b2e1e71c3318ba0518fe3b`  
		Last Modified: Thu, 30 Mar 2023 04:39:41 GMT  
		Size: 363.1 KB (363089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8b24f9438070c6ab529ee112a06a2e1977b8ad4d29346c3e6dbac9f2f2d9cb`  
		Last Modified: Thu, 30 Mar 2023 04:39:40 GMT  
		Size: 7.6 KB (7557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0187deee60d8aeabef55a6a1ef80e48ab121f0ada5f727166d9369521a5f15`  
		Last Modified: Thu, 30 Mar 2023 04:39:43 GMT  
		Size: 12.8 MB (12779922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:2d104000bca3541e5fff3b91ae1dac6e7f892f5465950d916c6e799f9dc44d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b20ebaa09fc779cb881f568b5ea4f787a57f40639951bd4c971eb392a6796dc3`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 18:12:20 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Wed, 29 Mar 2023 18:12:22 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 29 Mar 2023 18:12:22 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 29 Mar 2023 18:12:24 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 29 Mar 2023 18:12:24 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 29 Mar 2023 18:12:25 GMT
ENV XDG_DATA_HOME=/data
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 29 Mar 2023 18:12:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 80
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 443/udp
# Wed, 29 Mar 2023 18:12:26 GMT
EXPOSE 2019
# Wed, 29 Mar 2023 18:12:26 GMT
WORKDIR /srv
# Wed, 29 Mar 2023 18:12:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f4361b7a6ad780b98081afc006e9f731a690521551efa8322b8f84f987a3fc6`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 352.8 KB (352773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8db23a24af48e4d2e8fd1fad65d9536afee97e958b91d9c91b6ca07dd648e01`  
		Last Modified: Wed, 29 Mar 2023 18:12:46 GMT  
		Size: 7.6 KB (7555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8105ceb1cefbc03b3583795117a0b5ce54b2ed08ec19a7c8abeeb934f841441`  
		Last Modified: Wed, 29 Mar 2023 18:12:48 GMT  
		Size: 13.8 MB (13838806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:3f6d61ed02f8e689b02604b64416863fc5f161fe638e8facb43ed78e89849065
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4252; amd64
	-	windows version 10.0.20348.1668; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:dd8b35b944648b6de74e54e981624f78ee1745fa84d8c7a02bce54878668e019
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4252; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4252; amd64

```console
$ docker pull caddy@sha256:39a418c0cfa664f9b3688227376a2f3dafe49f67336252dad64e281d5abf2b98
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2086815958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8eb63ef752712fe8905e4f48738d35b3d848be3ef779a535db581758901f3286`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Wed, 05 Apr 2023 00:41:54 GMT
RUN Install update 10.0.17763.4252
# Tue, 11 Apr 2023 23:40:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 02:58:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 02:58:09 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:00:21 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:00:22 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:00:24 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:00:25 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:00:26 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:00:27 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:00:29 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:00:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:00:31 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:00:32 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:00:33 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:00:34 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:00:35 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:00:36 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:00:37 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:02:33 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:02:35 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9094c39c4b36a86359abb3da9e9d0d9c69b6930e9c7b308120310d43d63f693`  
		Last Modified: Wed, 12 Apr 2023 00:52:10 GMT  
		Size: 363.3 MB (363347289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9103f1e2cdefe8f16dae9619b88e38aa659abb17276d2362d435ad0721d3bf41`  
		Last Modified: Wed, 12 Apr 2023 00:50:55 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bab3ea41fadd01f5289d26cb8a1038721d52bb48ff08c216752ff741f4d9a4f`  
		Last Modified: Wed, 12 Apr 2023 03:12:19 GMT  
		Size: 515.3 KB (515260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f2dd85da1b91ed75a5c151a9c926b2e6d5b262e4d0e77ddcaab10277c9d8c2`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ae40a48d4f371751f918da00f2ad6485a6ffc55e3714df50831a25374c075`  
		Last Modified: Wed, 12 Apr 2023 03:12:22 GMT  
		Size: 14.7 MB (14675034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134ca3ec74859c043b3c5c1c7ffb1c477f9ef30b4a771d8970e4644021033396`  
		Last Modified: Wed, 12 Apr 2023 03:12:18 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8cb7378911c6c263b6c1cdbb78ba752555d6e8806e834456adc67eb82a3970f`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50a041cb220ee997f8bf50b6f4a8af12bdbbaf9b6b60796a2cba415ef4971f4d`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cde958705c423722a103e5fe75111b31ff6ee1e38b70fdca0da21f8723360b`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fe1869d94955698fc5e2a200e686b6b488b8e57850ed8b9cfbde6f636c33e3`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d80b46748483116877a3348aa54048b15e5148b25280017d70d590960b74122`  
		Last Modified: Wed, 12 Apr 2023 03:12:16 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e1a74657e24b09f672fa7afdcaa3b6c622464ec3e8a23986028cc1898c50f`  
		Last Modified: Wed, 12 Apr 2023 03:12:15 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f4bb45ff60a21ca007e50b817bfdf9c6c2771c9d360995b67d4294ace4cc0a`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1082d972bae2b72c59c9b5f5007b2b364f20fcaa345326b6fa81cf578b5f17c`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:641886c0342573c6e0d621e1e7fe90358ac08d6b06ad1fd0da4d69c4fdf71508`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517d0b81cf6bc91d7c2d91089f84e0b21b7a3aa666d77ccbcd5b2218ff31f76f`  
		Last Modified: Wed, 12 Apr 2023 03:12:14 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c80f14175e989e572a6139e5b7da56362ce2aa1a042f0c31443ee244ee7e674`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22a960dca640dbdaf57055fa493bcef4c88cfd57c100250e5b2c100eecf69973`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dc99769935623de3322b6378e4ec07c7b68598b466a71189aa41163c2862cb`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9878c0a96731fdc73d90bd3d36d06b2284b6f8587737e4babdc739d3e4ff0c`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 310.3 KB (310346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5025fc82d5d8be754b5f3444937f4425c25df7f1215a75a1b33d10efc7e4d0e`  
		Last Modified: Wed, 12 Apr 2023 03:12:12 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:85e9a8d2824c1d06afd808a980707fa129a3a734da68abfcbcb91733acdd0d29
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1668; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1668; amd64

```console
$ docker pull caddy@sha256:5816dd2cf3dc05cd0c9019779fdfb0f66bef2db535fe50bf9a611727d4973f0f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1778637888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:098f470930922cda98c57d068ebbd67a9cfe78f74d24540871d7187814631650`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Wed, 05 Apr 2023 00:38:27 GMT
RUN Install update 10.0.20348.1668
# Tue, 11 Apr 2023 23:37:41 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Apr 2023 03:04:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 12 Apr 2023 03:04:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 12 Apr 2023 03:05:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 12 Apr 2023 03:05:38 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 12 Apr 2023 03:05:39 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 12 Apr 2023 03:05:40 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 12 Apr 2023 03:05:41 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 12 Apr 2023 03:05:42 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 12 Apr 2023 03:05:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 12 Apr 2023 03:05:45 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 12 Apr 2023 03:05:46 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 12 Apr 2023 03:05:47 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 12 Apr 2023 03:05:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 12 Apr 2023 03:05:50 GMT
EXPOSE 80
# Wed, 12 Apr 2023 03:05:51 GMT
EXPOSE 443
# Wed, 12 Apr 2023 03:05:52 GMT
EXPOSE 443/udp
# Wed, 12 Apr 2023 03:05:54 GMT
EXPOSE 2019
# Wed, 12 Apr 2023 03:07:07 GMT
RUN caddy version
# Wed, 12 Apr 2023 03:07:08 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ecfa9c953d28a9da9d422b57cd0361c57c44e1faaaed7e50a2537d1c29cee1`  
		Last Modified: Wed, 12 Apr 2023 00:50:33 GMT  
		Size: 376.6 MB (376573004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98474c9b39bb0e3a2d79dca81a90952011b65d1fa352021dacd30335d1bb69f4`  
		Last Modified: Wed, 12 Apr 2023 00:49:03 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b471ee71b60190b36c6532e53c505ab1de93aa7c9e51c7bebe3bb06f38962dc3`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 777.4 KB (777408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e982886e5454b0a89f3a890f8686717d267de222d97aa28e9b965b2757df5ff0`  
		Last Modified: Wed, 12 Apr 2023 03:12:47 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdd51977aadb15096291fc41a2d0337d36ee689de0cd9c276695fb5197c50aa`  
		Last Modified: Wed, 12 Apr 2023 03:12:51 GMT  
		Size: 14.9 MB (14886500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d7531b8f393c29502558d55f39c55302333c06222efeaa7f419446a222f337`  
		Last Modified: Wed, 12 Apr 2023 03:12:45 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160c04fcb4a5bffea4d80d2867e6fcac489dcbf8c4a35d5e85a67a929c888ef9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0784b592b7e3f2b494c71f279147da7c266341fb0587a5c59bbfc9e41dea77d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f9cfce69a9c6d6b6b3007e9b0c7448058d74509602e22fec75861878c0742c9`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d4b3de2f22a6fce7c825b986b588cc14c0b7c67cd7178e1506f6352847af6d`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab54cdbb657929c562f49244d9e0492bfb404a8095486b79fd2d3ecbf6bb1a38`  
		Last Modified: Wed, 12 Apr 2023 03:12:44 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b018dd2781aae0f25de0b285ade187c0f4397a3d5ffb41ba9c6929130e280f`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c20d583cfbaaf94ed46365e5e18be9d9acbd7b787d11b8564a96f2eb0b4c292`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97118f2089bb3729cf5818e640b334bf01f42bdcdb873ec2a28c9456abc12fce`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90c9ea843613874c055678636826a2021322f141bb478e0bc42cbca0b5ada97`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0009c0e106f18410276bcedf8cdd092320bf7d55d650b83eef76f2e861271d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:42 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e00f14f7cce82dc703004137c80e446f6153540fca1ffd80b77b139f12e3666`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5555a21ba1a23ae8957bd7f220a308f42ff9b9643920f1966f3a6c6328a617a5`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b073e21b86b0217d0b53c328e53066bbc1956dd703ec27016e31d27d726943`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df47667114448a2e54bda68d712745488b3be05b7f8ac4f053181232f2bf9fa0`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 347.9 KB (347888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ef65483af329350882b60ca40f74069115adcc9564135596fbf78abeb21a2d3`  
		Last Modified: Wed, 12 Apr 2023 03:12:40 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
