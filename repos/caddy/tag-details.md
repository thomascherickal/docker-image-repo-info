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
$ docker pull caddy@sha256:bc23ee7f830ab9d029e5469e82a3e36f8c401001c2c8a5a6d919a82668d8087b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:4dfec6c3b22c36b63ea4a3633c7cdbdaa9926d1324c27db2b0e2b70ef9cd105a
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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:6bf3c895704ceba8561ff1d0cb761476cd488ae27b0593be332b923be6c65a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:6c6f74c0b96dda41269a52cc0fb8e0e5e84bbaf5e6ffb8b90e5139c87e4afab4
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
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fe09db48db55efa25c43c2664ffe869f89df9d49dab78bd30d676808554fb9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25f672a5954947c8808d8d3801c159b53ce37657e8877f3c1b193e157f32f305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:98966406b58f67077e5f9f7777af422b5d457b111c57af42011679fedf887d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:b3415e2370c025a924067cb08c32af70dcab6b8df5f5da24eb74948c0b56cb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:89cf400670f4d5e7722ebc4ec20a3b712b53af6b3a1d003884656d4069a43098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:bc23ee7f830ab9d029e5469e82a3e36f8c401001c2c8a5a6d919a82668d8087b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:4dfec6c3b22c36b63ea4a3633c7cdbdaa9926d1324c27db2b0e2b70ef9cd105a
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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder`

```console
$ docker pull caddy@sha256:6bf3c895704ceba8561ff1d0cb761476cd488ae27b0593be332b923be6c65a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:6c6f74c0b96dda41269a52cc0fb8e0e5e84bbaf5e6ffb8b90e5139c87e4afab4
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
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fe09db48db55efa25c43c2664ffe869f89df9d49dab78bd30d676808554fb9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25f672a5954947c8808d8d3801c159b53ce37657e8877f3c1b193e157f32f305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:98966406b58f67077e5f9f7777af422b5d457b111c57af42011679fedf887d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:b3415e2370c025a924067cb08c32af70dcab6b8df5f5da24eb74948c0b56cb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:89cf400670f4d5e7722ebc4ec20a3b712b53af6b3a1d003884656d4069a43098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4`

```console
$ docker pull caddy@sha256:bc23ee7f830ab9d029e5469e82a3e36f8c401001c2c8a5a6d919a82668d8087b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-alpine`

```console
$ docker pull caddy@sha256:4dfec6c3b22c36b63ea4a3633c7cdbdaa9926d1324c27db2b0e2b70ef9cd105a
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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder`

```console
$ docker pull caddy@sha256:6bf3c895704ceba8561ff1d0cb761476cd488ae27b0593be332b923be6c65a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-alpine`

```console
$ docker pull caddy@sha256:6c6f74c0b96dda41269a52cc0fb8e0e5e84bbaf5e6ffb8b90e5139c87e4afab4
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
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fe09db48db55efa25c43c2664ffe869f89df9d49dab78bd30d676808554fb9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2.6.4-builder-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25f672a5954947c8808d8d3801c159b53ce37657e8877f3c1b193e157f32f305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore`

```console
$ docker pull caddy@sha256:98966406b58f67077e5f9f7777af422b5d457b111c57af42011679fedf887d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6.4-windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:b3415e2370c025a924067cb08c32af70dcab6b8df5f5da24eb74948c0b56cb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:2.6.4-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:89cf400670f4d5e7722ebc4ec20a3b712b53af6b3a1d003884656d4069a43098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:2.6.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:4dfec6c3b22c36b63ea4a3633c7cdbdaa9926d1324c27db2b0e2b70ef9cd105a
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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:6bf3c895704ceba8561ff1d0cb761476cd488ae27b0593be332b923be6c65a48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:6c6f74c0b96dda41269a52cc0fb8e0e5e84bbaf5e6ffb8b90e5139c87e4afab4
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
$ docker pull caddy@sha256:bbe9f7e2106c8954433b179563da0124860629d757c0eb85c1a37cb91e4dab0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.3 MB (132253065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecbc353690b010ceb2bfb3cf689d380cbfb65744b4353acd6262482c3d681229`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:10 GMT
ADD file:7625ddfd589fb824ee39f1b1eb387b98f3676420ff52f26eb9d975151e889667 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:10 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:27:41 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:29:39 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:31:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:31:15 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:31:15 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:31:16 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:31:16 GMT
WORKDIR /go
# Thu, 11 May 2023 21:19:39 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:19:39 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:19:40 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:19:40 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:19:41 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:19:41 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:19:41 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:8a49fdb3b6a5ff2bd8ec6a86c05b2922a0f7454579ecc07637e94dfd1d0639b6`  
		Last Modified: Tue, 09 May 2023 23:11:26 GMT  
		Size: 3.4 MB (3397490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58116d8bf56953e5f30b7f50257c5bb2b5ba4aba460cb69f2ac57eea00aaa5dc`  
		Last Modified: Wed, 10 May 2023 00:00:24 GMT  
		Size: 284.7 KB (284686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fb277e54df7c9e15c16f2958c8b8efa9d62c7375bd6a32a30507c9fc1da8be`  
		Last Modified: Thu, 11 May 2023 19:32:43 GMT  
		Size: 122.4 MB (122403920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2302f1b49b03f3e04f5c752e81534fadc9b2fb6ae6d7ccb354000e720c55eb87`  
		Last Modified: Thu, 11 May 2023 19:32:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f125368af659a05cab9d286b251e172f13c6e26a790ee4378c0dbd5c033380`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 4.9 MB (4948575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6958c4d5df2be656149a30334db272a7591e9a9f259f14aa7b68ec3e967bf90e`  
		Last Modified: Thu, 11 May 2023 21:19:55 GMT  
		Size: 1.2 MB (1217834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e012d017463f26e62b6959a9e965f4aaaa91f39bcb0a77e315d2fb4a544d10`  
		Last Modified: Thu, 11 May 2023 21:19:54 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4c80ef586657fb74f7a185d0ca14639ed15778d1ed00e5c8e0f6bc548918d268
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128320428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a88b73965f9dcda34a1c12113511b62f8c4117a65ea9646ca909b3471e3340b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:04 GMT
ADD file:f87a991e2e9f185fd4a88569d86a9b8e5bc07182e7fa613b95acab25986f2a6c in / 
# Tue, 09 May 2023 23:11:04 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:13 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:50:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:52:30 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:54:33 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:54:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:54:34 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:54:34 GMT
WORKDIR /go
# Thu, 11 May 2023 20:56:41 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 20:56:41 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 20:56:41 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 20:56:42 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 20:56:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 20:56:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 20:56:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:015ee8d9fb3dca1b18815f1e4ee0d325d1f40cde6f2df4dd307918f7b69167d7`  
		Last Modified: Tue, 09 May 2023 23:11:20 GMT  
		Size: 3.2 MB (3155679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a91154cf231582e0efd441a318760e357cccbcf664976f729d125fe63ccdc9`  
		Last Modified: Tue, 09 May 2023 23:59:27 GMT  
		Size: 284.9 KB (284873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7339eadee78af92dfd9c0ea9722438739bc76bad4e632e4c520c2d26542f6244`  
		Last Modified: Thu, 11 May 2023 19:55:47 GMT  
		Size: 118.8 MB (118774346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:790bf33efe0a479501b886102fe0398d3a28dee1328ee73dfb59eb1c9330f7aa`  
		Last Modified: Thu, 11 May 2023 19:55:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58228b8a3c7b3e5f1bfcfe003394b0df1bfab350ccc468af0fa2555abc644d38`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 4.9 MB (4938901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa2593c7d982c28414c3f96a0d57a064af82d05d8d8e2dcd9947e19fcbf66e6`  
		Last Modified: Thu, 11 May 2023 20:56:56 GMT  
		Size: 1.2 MB (1166069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11457c7696f2ddbf3af41b46f4c1678a0cc653e8bc3e634a0ff8f1cce663d4ba`  
		Last Modified: Thu, 11 May 2023 20:56:55 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:332ed0cc344b734114ebfb6ba505b9b4b08c9f5b98324bdf2e150d7cce49f551
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127389599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b544c8546a36cd72f1bf15e6b516049c89d29bfb65b7a46fb1c22cb8976f278d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 22:57:32 GMT
ADD file:eb6b6a885e8ac9bccbf44a5c673b8542c8144bba927376688240446c2f413b10 in / 
# Tue, 09 May 2023 22:57:32 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:07:21 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:57:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:00:05 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:02:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:03:01 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:03:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:03:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:03:02 GMT
WORKDIR /go
# Thu, 11 May 2023 23:18:43 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 23:18:43 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 23:18:43 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 23:18:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 23:18:44 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 23:18:44 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:e14425cf8fb9304b9ad4a9d1250e0d4c22e507a334ff747fa69b804500afc113`  
		Last Modified: Tue, 09 May 2023 22:57:50 GMT  
		Size: 2.9 MB (2911117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7807d1567ad70e9e42db0b7a4aa54ab9afc3df1c31c3fb590ced28192601e947`  
		Last Modified: Wed, 10 May 2023 00:07:35 GMT  
		Size: 284.1 KB (284075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b1085b8d763d7c84b599a740ef23721df45f5bcd0e2b590a6287cee492b402`  
		Last Modified: Thu, 11 May 2023 20:04:42 GMT  
		Size: 118.5 MB (118539285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae059e14f3773e6331a0c7f752d0d150b627141dec7030ea56614cae2a84939`  
		Last Modified: Thu, 11 May 2023 20:04:19 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43488c94b3b271d5725a29e7bb71ca026b536d9796f27051e34fa2f341ef7f49`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 4.5 MB (4491232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f55d821d30e73dd1cd37e500e09f0cb7e9f6f2750560f2b0787dd135e4ddf32`  
		Last Modified: Thu, 11 May 2023 23:18:58 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec6e4688765e457aef04e6dc303251a7790a40a91b963803ebaa45d3eb82396`  
		Last Modified: Thu, 11 May 2023 23:18:57 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7eff8bc556d8a73cb183dfe7fa8df65846a03776f18f36b5b0741b5b9d6a6513
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.8 MB (126774669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43f4c1a2d87bf206b6eedf6a3e26795c5025e36eb6ab24425afdec0c9653af37`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:08 GMT
ADD file:df7fccc3453b6ec1401d27a1295b0882a83e731fde8f23db9d3f687a2b6b4e70 in / 
# Tue, 09 May 2023 23:11:08 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:03:32 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:46:01 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:47:13 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:48:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:48:25 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:48:25 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:48:26 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:48:26 GMT
WORKDIR /go
# Thu, 11 May 2023 21:38:13 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:38:13 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:38:13 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:38:14 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:38:14 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:38:14 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:08409d4172603f40b56eb6b76240a1e6bd78baa0e96590dc7ff76c5f1a093af2`  
		Last Modified: Tue, 09 May 2023 23:11:23 GMT  
		Size: 3.3 MB (3342848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8683203a1cdbff667eb41c5b6d8426e77bcb98ede7a1aaf8def0259eab83f01c`  
		Last Modified: Wed, 10 May 2023 00:03:46 GMT  
		Size: 286.3 KB (286287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce7fc06b337e365feb0fd5ab053ffbd925b7e960f8936f5dda0f345456dd91e`  
		Last Modified: Thu, 11 May 2023 19:49:38 GMT  
		Size: 117.0 MB (116978981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6733b0a33a3e922a921293d18546a29e44cb6c0a43e0ffa426fb129ec7232336`  
		Last Modified: Thu, 11 May 2023 19:49:26 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec4a0193569a98c3088593f0589d1afe9a3570cd82f991d862da441371a34cf`  
		Last Modified: Thu, 11 May 2023 21:38:37 GMT  
		Size: 5.0 MB (5042258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3ee5b2f6d2acf1b1261f01868982782145243f6662148a6becf1325e79c53a`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431fe740c562a43a89708a424fd6e6c135d27d6e5b7bf086c6b092085fecac8b`  
		Last Modified: Thu, 11 May 2023 21:38:36 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d9178dd19798e764e7cc1ec9331a3e9a351295937a77113b66c39569fbb3dd69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127371269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:968da7c905e323d46479d982724619f80859acbc989085fca7678b556f642641`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:09 GMT
ADD file:0a227602737a24c596923d3fd0a7c8b7d9000dbc6b80561473def09abbebbfa6 in / 
# Tue, 09 May 2023 23:11:10 GMT
CMD ["/bin/sh"]
# Tue, 09 May 2023 23:59:39 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 20:16:32 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:19:46 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 20:22:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 20:22:45 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 20:22:46 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 20:22:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 20:22:47 GMT
WORKDIR /go
# Thu, 11 May 2023 22:43:52 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 22:43:53 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 22:43:53 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 22:43:54 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 22:43:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 22:43:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 22:43:58 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5c0986f188e93dd7e76a4dc49a9170da2cd124709f5e1590b378e31a2b0d9587`  
		Last Modified: Tue, 09 May 2023 23:11:31 GMT  
		Size: 3.4 MB (3385631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376ba25ac41cec041d831e456ad293ec2efd7e4fd1357ae113210bfddd447a5f`  
		Last Modified: Wed, 10 May 2023 00:00:00 GMT  
		Size: 286.7 KB (286653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c95502e7a529091c8fae8ca203e67f3a92268b55d487c20b53ef7d13fb044a8`  
		Last Modified: Thu, 11 May 2023 20:24:28 GMT  
		Size: 117.3 MB (117349132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681dd31d47c651e7e419f540426af2b84f2afc03e5c81ccbbcf34cad7b94a656`  
		Last Modified: Thu, 11 May 2023 20:24:00 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8e96ef9baea077f411d0d0534ee906b62009758f0ec4d87693cd3a2208f403`  
		Last Modified: Thu, 11 May 2023 22:44:16 GMT  
		Size: 5.2 MB (5243399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e3613535a15a886cce467c7bd91705d093aa295b5142c84c289e99de49c7f80`  
		Last Modified: Thu, 11 May 2023 22:44:15 GMT  
		Size: 1.1 MB (1105893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510acd116b9e81faacbc2e6fd6f669fe6d6b1b73299b9b48127a04feebd29090`  
		Last Modified: Thu, 11 May 2023 22:44:14 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:0592cae8bb3f62fcc5e3b8cabceda28e9a0327fac67c82b8561978ad556d21e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130625542 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bef10faa1b046c54ced82c5b5fc71bf4db82bf52fe8eaa5f3ff8cf365f140bcb`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 May 2023 23:11:06 GMT
ADD file:89d6e366e8ab41011a5866f8ca43aac6cfef00edffebad565918ab632a6d6210 in / 
# Tue, 09 May 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Wed, 10 May 2023 00:00:53 GMT
RUN apk add --no-cache ca-certificates
# Thu, 11 May 2023 19:41:59 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:44:12 GMT
ENV GOLANG_VERSION=1.19.9
# Thu, 11 May 2023 19:46:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.9.src.tar.gz'; 		sha256='131190a4697a70c5b1d232df5d3f55a3f9ec0e78e40516196ffb3f09ae6a5744'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Thu, 11 May 2023 19:46:16 GMT
ENV GOPATH=/go
# Thu, 11 May 2023 19:46:16 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 11 May 2023 19:46:17 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Thu, 11 May 2023 19:46:17 GMT
WORKDIR /go
# Thu, 11 May 2023 21:13:17 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 11 May 2023 21:13:17 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 11 May 2023 21:13:17 GMT
ENV XCADDY_SETCAP=1
# Thu, 11 May 2023 21:13:18 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 11 May 2023 21:13:18 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 11 May 2023 21:13:18 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:25da54cc0a08f4ca602c6bcd3e52d70082eb8a25ee022bc9f1dda019de49197a`  
		Last Modified: Tue, 09 May 2023 23:11:35 GMT  
		Size: 3.2 MB (3226303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a72fc573296d33547281b8f37ff15a477a2844bdd1fff61bf191b5f18e14354`  
		Last Modified: Wed, 10 May 2023 00:01:13 GMT  
		Size: 285.1 KB (285083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea123020274bbdb184bcd47d98c6f33c76dc8b5566fe97398548e786eb161d`  
		Last Modified: Thu, 11 May 2023 19:47:34 GMT  
		Size: 120.9 MB (120855414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208d8e7e4406cfc1abe11afab0d01281fe0493debaa9f1099ca1a16607aa365e`  
		Last Modified: Thu, 11 May 2023 19:47:18 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb63ca2f81985ab2cb6faf2347639a1079fd5e025f077ddbbf54a5f7d612b96a`  
		Last Modified: Thu, 11 May 2023 21:13:38 GMT  
		Size: 5.1 MB (5087764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ddd73e4f3b21578f6786a9fe3dbd4e3ab5ed24a128bbf3475fd151f39e695c`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 1.2 MB (1170418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ef8cbc2da4dfd04998249e67beb35985d9ba5e8cd2c9e4570c5ea926920b19`  
		Last Modified: Thu, 11 May 2023 21:13:37 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:fe09db48db55efa25c43c2664ffe869f89df9d49dab78bd30d676808554fb9cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:4f209487a80ee67e3441517504b04fef7cdd87394f6d9b25020b5d1041cf6ae9
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2257120122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45212d196c9e6368b4c4441dfcc4749161225c56588720c7b7b89394c086404`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:22:55 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:22:56 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:22:57 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:24:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:24:15 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:25:19 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:36:16 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:39:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:39:28 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:08:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:08:43 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:08:43 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:44 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:09:50 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:09:51 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69c8e1c8adec95ce194194fafcfc6a1e07f15344588a0b08f7f625c5a547434`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47736757cd8e844fa5669cb79caf4053a95eb6b57e09dd4ab01823f071f92f24`  
		Last Modified: Wed, 10 May 2023 01:46:45 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfd4aa96423c060d9cbb5c55c535627e8c1e46ba89f752a3d601450afe81b5b8`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077f8de560673af047f7136635e2e62927f8f69d11a928140de06383e86fb295`  
		Last Modified: Wed, 10 May 2023 01:46:44 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed8138b5cc05a953f350e06a0713c2c031257b514bb362629f520d00db71fd7`  
		Last Modified: Wed, 10 May 2023 01:46:49 GMT  
		Size: 25.5 MB (25530178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814a31d39859b5f50d901390aa5410b00f1637dce1a5839d12e69722fab50294`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e05276aaa698fd9d43e2a1961637e16578fa84a5128237d7c2bdfe57c54fa89`  
		Last Modified: Wed, 10 May 2023 01:46:42 GMT  
		Size: 262.2 KB (262162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecdb7abe61438b7c484538d9abcbf9f221e8250bbc14ff0340952477872ca8`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8a8051e6917bcca154f994e561aaca88eec8542d26c4215449c493cc20677a9`  
		Last Modified: Wed, 10 May 2023 01:50:27 GMT  
		Size: 157.7 MB (157699831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819570cca8314d2c43127f47e580ccca379d28ee2b2a710a0cf56ac3dc22e5a9`  
		Last Modified: Wed, 10 May 2023 01:49:56 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb1cac98386c21a9acf42c96ef5775a0f72c5d8aa5b0d4702c8878a59324521`  
		Last Modified: Wed, 10 May 2023 03:12:06 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea0b2ad2f8f246a1ca082b0d8743e50c3d55ca2c0285cde692ecc38722fd9cb`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006fe2de64e8f1d2558c43ad0a9b14181aed1de7768c87f9d574b65a3f3bd715`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f7fb0bdf9bd756aa0059205239715bc0a7e8b3b42eb71f1ac6abe754defcc`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5153750f7b220df006ddff9296efc22eca6f44606ff7f7e491b2352530388194`  
		Last Modified: Wed, 10 May 2023 03:12:04 GMT  
		Size: 1.6 MB (1575044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb86d9dfa76a5b87af8edf4871150f51a4ce317790606fb471678ba96fc278d2`  
		Last Modified: Wed, 10 May 2023 03:12:03 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:25f672a5954947c8808d8d3801c159b53ce37657e8877f3c1b193e157f32f305
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:e5b19e5a934f5f4e06ab7d8ffc01521ccbb247d70dff6f52a26564b10c891742
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1960073641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d023e4040491ea2712124498fc29d55b3cf7919521b1b2a11cdbcabc9a413a2`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 01:19:25 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 May 2023 01:19:26 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 May 2023 01:19:27 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 May 2023 01:19:59 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:20:00 GMT
ENV GOPATH=C:\go
# Wed, 10 May 2023 01:20:22 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 May 2023 01:33:33 GMT
ENV GOLANG_VERSION=1.19.9
# Wed, 10 May 2023 01:35:57 GMT
RUN $url = 'https://dl.google.com/go/go1.19.9.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '3b0ca22aedf5fd85e84c944dd96ab3044213bf224cc3e9850ad86f1f71e1be93'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 10 May 2023 01:35:59 GMT
WORKDIR C:\go
# Wed, 10 May 2023 03:10:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:10:10 GMT
ENV XCADDY_VERSION=v0.3.2
# Wed, 10 May 2023 03:10:11 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:10:11 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Wed, 10 May 2023 03:10:35 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Wed, 10 May 2023 03:10:36 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a5817a4fb4758348ab4368724df2dc391387df461e1a8d85ce78b44e62941c`  
		Last Modified: Wed, 10 May 2023 01:45:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dab590dc88f85f33daec526784c193cc1c9b17e7b5698c2c2062f2834024c6`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f079b4dc01fb29bd7fef59856746267beedc000a15ee3384aae24b0611e20ca5`  
		Last Modified: Wed, 10 May 2023 01:45:24 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079e97ba795ef33077d3adec29756d746b1770b10fd4625881edcef794037e1c`  
		Last Modified: Wed, 10 May 2023 01:45:23 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb79b38ccc75aeae87db4cf726d0dca1e9d555cd554c4556b9968117ef8f7cbf`  
		Last Modified: Wed, 10 May 2023 01:45:28 GMT  
		Size: 25.5 MB (25531790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cd856add23470d3d95bee9f5f2ece447db6ec28e58975639ca4a4d7633ca09b`  
		Last Modified: Wed, 10 May 2023 01:45:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e2692a8e8e09064af3cb6bbd4e5562607b52cf8ed9fa0aa22c9bc50a7117ae`  
		Last Modified: Wed, 10 May 2023 01:45:22 GMT  
		Size: 264.1 KB (264060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e7b94c7f60d806263cffec1d505889ddaccda18f2c2c06e16868b4aaf341d7d`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.4 KB (1372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9476426358feedd380d165a6545784aefbacfc6d43a1adc6a8e0b96823d0695`  
		Last Modified: Wed, 10 May 2023 01:49:47 GMT  
		Size: 157.7 MB (157701502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f264d31923b50e5e899fe038e9e11527cb4317ca3048d06d673214ed013d641`  
		Last Modified: Wed, 10 May 2023 01:49:15 GMT  
		Size: 1.5 KB (1454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70ebce5d2af36baa0e1fc61e0f643f9a03a38733584ff68816220fba97dd53e`  
		Last Modified: Wed, 10 May 2023 03:12:24 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df3ce860673aedeb90b4289c7c4b2bfbcb6c71c50986459deca538704647a889`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d8999d96f9d031dcd80d0f7a32d120bf3ab1da692569aa7024eb4040066631`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9e094429f042b540cb1d80bcd14898a6961f69b4daf95c690c272c6e731535`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6136ef5d6423b5a9893c858e7d25aa3b035adba5002362a26bb37b8a26327e`  
		Last Modified: Wed, 10 May 2023 03:12:22 GMT  
		Size: 1.6 MB (1577446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f9dd1eb1a6a5d6a401cce31fd6a16b851fe2e0de89039b33499ebb00a60702`  
		Last Modified: Wed, 10 May 2023 03:12:21 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:bc23ee7f830ab9d029e5469e82a3e36f8c401001c2c8a5a6d919a82668d8087b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

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
$ docker pull caddy@sha256:2a8d2350281c0b34e785a3822691c36f0d13e1a82038999f993ceaaeb903d652
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.8 MB (16792548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a1dee5e3b9e398104c8af3eb418c10a7603849782d837613c4cafe9aca18346`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Wed, 29 Mar 2023 17:42:02 GMT
ADD file:6c3b2d8f192a3a12e6df8bc7130bbc723b1a39aa71809d23b15cf80bc5135096 in / 
# Wed, 29 Mar 2023 17:42:02 GMT
CMD ["/bin/sh"]
# Tue, 02 May 2023 19:12:39 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Tue, 02 May 2023 19:12:40 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Tue, 02 May 2023 19:12:41 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 02 May 2023 19:12:44 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 02 May 2023 19:12:46 GMT
ENV XDG_DATA_HOME=/data
# Tue, 02 May 2023 19:12:46 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 02 May 2023 19:12:47 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 02 May 2023 19:12:48 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 02 May 2023 19:12:48 GMT
EXPOSE 80
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 443/udp
# Tue, 02 May 2023 19:12:49 GMT
EXPOSE 2019
# Tue, 02 May 2023 19:12:49 GMT
WORKDIR /srv
# Tue, 02 May 2023 19:12:50 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:95cbbfdf0c760cbcde91603c8eee15ec60d4aa5f874b4a538babcd2df1709174`  
		Last Modified: Wed, 29 Mar 2023 17:42:37 GMT  
		Size: 2.6 MB (2593389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67198d339fb89cea75684337f899057b33b31485993389f2b580d32bc2049bca`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 352.8 KB (352796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e681c779f6227da94de2c84d6c813597a989bf4818df00dea18da899298abfd5`  
		Last Modified: Tue, 02 May 2023 19:13:18 GMT  
		Size: 7.6 KB (7560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252df245f95deab402a183510f19ee42e7bc7181cfc7d295c5c6c0385b066624`  
		Last Modified: Tue, 02 May 2023 19:13:20 GMT  
		Size: 13.8 MB (13838803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:98966406b58f67077e5f9f7777af422b5d457b111c57af42011679fedf887d80
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4377; amd64
	-	windows version 10.0.20348.1726; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:b3415e2370c025a924067cb08c32af70dcab6b8df5f5da24eb74948c0b56cb0e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4377; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4377; amd64

```console
$ docker pull caddy@sha256:bf1f9b05cd873cf00fb889174804fc09871d536192e28ca79806d2ce06ac8be7
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 GB (2087375418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8bf96c22a8f8ca00c7b1aa4ea6aa818aaecc66be8cc1041ca0e601e7a505371`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Fri, 05 May 2023 12:05:28 GMT
RUN Install update 10.0.17763.4377
# Wed, 10 May 2023 00:36:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:04:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:04:27 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:05:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:05:46 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:05:47 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:05:48 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:05:49 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:05:50 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:05:51 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:05:52 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:05:53 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:05:54 GMT
EXPOSE 80
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443
# Wed, 10 May 2023 03:05:55 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:05:56 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:07:04 GMT
RUN caddy version
# Wed, 10 May 2023 03:07:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01de39a0c44e24aa1912078d32ee54389b71154e509138cc4f5d1de42e7a32a`  
		Last Modified: Wed, 10 May 2023 01:47:41 GMT  
		Size: 364.1 MB (364091294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a238e462da347b2e29386c9883c0ec93c8dbce311782ea1c5abbec2a31d884`  
		Last Modified: Wed, 10 May 2023 01:46:46 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ccc021a0ffd29ac554311786b18ef3f4ce79304b32b3987c4b15d76740eb7`  
		Last Modified: Wed, 10 May 2023 03:11:20 GMT  
		Size: 452.1 KB (452128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698181b72cdb77e36337a00405b68dda39d3d2cd554f8c58224bf449c9e6434`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45ad734018db3b416d9411409fbf4b1fd962fc86b9f084f29178553e9a02893`  
		Last Modified: Wed, 10 May 2023 03:11:22 GMT  
		Size: 14.6 MB (14606465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fba1db5304dd13aa3c829c71db3499b7654768728d5ca7b6a614cea47117b80`  
		Last Modified: Wed, 10 May 2023 03:11:19 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05bb775df753b9925f91b7a73e710b06b08c4bab0a4a99edf0207ec064cb7412`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:249cd1a03b939f74fd9fd25469cd0f680d23c21a538acd06e817e122ba76544c`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aeb63434040f9b9d6731d4256c2260add6ef6abc2d76a373b93ba2c0ad1af1e`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbcc40645db58161e5f421fc5743065ea5b0b855b7f43e1ff7e56b89a9ad5ff`  
		Last Modified: Wed, 10 May 2023 03:11:18 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae32c8eab142d3066a0e3a2cfdb1566684854bfbd41b881a369ba40644d733`  
		Last Modified: Wed, 10 May 2023 03:11:17 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9976933db5878bd15e571a3536a9599e7f03669308d0f8387483d1f2e64b04`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05192cfb3bddb797a27af99f4b20f980ec3d66d94fb339aa5e05e7628458d0ba`  
		Last Modified: Wed, 10 May 2023 03:11:16 GMT  
		Size: 1.4 KB (1447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2b54eaa5aa52b3cbfe07b57bcf6db822d260bbe7d08a8b5831900ed9a0aa33f`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a91c50af884ce4981d30938663f16959a892f71f3ca95077dbc2e7466ce8250`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87549b93f6723fa765b96b3f028e82cf7269edf04a813ceb908ef4ab0d8398c`  
		Last Modified: Wed, 10 May 2023 03:11:15 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3de8ba969ad5d4b84f4189ccbae6a41d8762556d6bdb747dbd96c17f4a36cc`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe06f9a0fde1b305c1c1984e3c5d329e25ae772ad6d97aa8d831337008eb95dc`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2d3002142e2b1d73a3caa9378851a440a5066afdfe4fbce0d782d12131f016`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:388f0b8cd9044e8da9a81b2b3521d00cbd4c9c3a5fc34bb930e933697b68c665`  
		Last Modified: Wed, 10 May 2023 03:11:14 GMT  
		Size: 258.9 KB (258943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc3ebc8e7d4a1c8f142db40262181ea8c803b37e889ccec8fda30d53a195541`  
		Last Modified: Wed, 10 May 2023 03:11:13 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:89cf400670f4d5e7722ebc4ec20a3b712b53af6b3a1d003884656d4069a43098
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1726; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1726; amd64

```console
$ docker pull caddy@sha256:929c50a8b4791c54f2e1639de794e8cade548d61988712dcd652a95402d0148d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.8 GB (1790344533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a221d4a4493c65a6549080916a8f547a1f2a2981be502861ccb9f1c1a51fd6`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 05 May 2023 13:22:05 GMT
RUN Install update 10.0.20348.1726
# Wed, 10 May 2023 00:35:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 May 2023 03:07:37 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 May 2023 03:07:38 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 10 May 2023 03:08:03 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 May 2023 03:08:04 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 May 2023 03:08:05 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 10 May 2023 03:08:06 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 May 2023 03:08:07 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 May 2023 03:08:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 May 2023 03:08:09 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 May 2023 03:08:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 May 2023 03:08:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 May 2023 03:08:12 GMT
EXPOSE 80
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443
# Wed, 10 May 2023 03:08:13 GMT
EXPOSE 443/udp
# Wed, 10 May 2023 03:08:14 GMT
EXPOSE 2019
# Wed, 10 May 2023 03:08:33 GMT
RUN caddy version
# Wed, 10 May 2023 03:08:34 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5829cfc8807e3c8e6f804ec45e3696c2b2e76cd39141b9c20486f8f070f56002`  
		Last Modified: Wed, 10 May 2023 01:46:28 GMT  
		Size: 389.0 MB (388952384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d178a10e123ab9f41a66d7e6d8ffca4aab5fba57cf381f48bc0090f603be2d5`  
		Last Modified: Wed, 10 May 2023 01:45:26 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1dfab80f3867c60027c22668e653f31ee742f2aff9a657e77b855d6f51661a3`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 459.6 KB (459571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3079f1dcb64f7fcae00920211fb4825bba7021097f0386c8889f8abd2de0afc8`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3e9b770b2b02ddb5444464dffe7e26e2e7b85aa27ef3a1ad3bde1df06b65be`  
		Last Modified: Wed, 10 May 2023 03:11:47 GMT  
		Size: 14.6 MB (14600557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1b2e5deebd7f73e0863a9cc5ad2ce5ecf323adf68acf42ae7529888174425e`  
		Last Modified: Wed, 10 May 2023 03:11:44 GMT  
		Size: 1.4 KB (1383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16aa7b98f1423486f61bb66f669a1d68890f2b087c6ed05733ed885072464e5f`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a737c90bed82468fcdca0e060b2daa988dd1fa07e991d411e6b83b31e8e2834`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a20e8e22af7793fccf98b3a305f6f81d8d677304324a2e5d14799b9a1d63a2e`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269d951fc3108478a270cef2581aa13e0cd0d52f5c78c746f832f799a18e30ed`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cad00ca38c4b688756162b907b83786ed67c2ce4ceb0a128ea72c5d94e87cac`  
		Last Modified: Wed, 10 May 2023 03:11:42 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d852aadcf908726f1ba182902404b8c3d3ab909c3b3113b419d97a18216d702`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598308b20e6c84ceccd195db3d39deba643146441a4acfb493217097cd014204`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412a41fcc9167f70a4565e36537175b5cf0fa9bda837628e49557157395ab5f7`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fc7647875ee9a754e92252085531d90a059b1c6cefb18e11c78860f22253ca`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52e570f0df18e5c6c644eaaf01cf018b513b07d6c2973ea3466df1bd2062e06`  
		Last Modified: Wed, 10 May 2023 03:11:40 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69405d2e06cce01af8a4c42683e46b7f8e12a77e142fe18b98e1035e9b1361a4`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4cf0a988af8b05d81f53ad816a88a0d5b5a6a6161f66bbc65758bcfa75fd031`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c9fbbf07055006f2ed39c071ec436539ef113505937535078b62f9a1bb762af`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442079b7e020642a4fe77d0d3fdf89b293fedda2d19f4e7039fe3f23fd9bd7dc`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 280.5 KB (280508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12468fe648f4487b224b87329712c50426783ab598281fb7e664095788354456`  
		Last Modified: Wed, 10 May 2023 03:11:38 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
