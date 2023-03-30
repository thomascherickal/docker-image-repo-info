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
$ docker pull caddy@sha256:6b9c77b69da1cfdaa859416f1f6dc8f1af4c615e548bd7278956876134dc3244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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

### `caddy:2` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:d3e698bba2b53f43485241c9c8b87a48f34017f31adecf925fefd176d60b8422
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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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
$ docker pull caddy@sha256:2d25080ffc0c6a95bf450c4103c28eeda17d212c1b4e550fa5ecc3572c9d1c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:c3f639c81b0fbb4b2d9d83345a6369dce5b90f3807c6f8474a2c2f2e3d5c969a
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
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:907bcf6ffbd9c87d579d9fd0c863633d3d5d3a4f7bbbe941849c977bcb479c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:2e8a4be822107da84510e9420e45153402e0561172b7d440cc58d9e42282e59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:92e187efa2c1a4f653fe84781b9a61f067ecea93ec473084a2e54f46283c8db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3ebcc75c760fd3f09c9af3a083679243b86e38acac6b9c87d426f5e060bb5e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8b07fddd6e884d7cd57b16fe8dfc8d764e50c606b804ace49eac539534eba9da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6`

```console
$ docker pull caddy@sha256:6b9c77b69da1cfdaa859416f1f6dc8f1af4c615e548bd7278956876134dc3244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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

### `caddy:2.6` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-alpine`

```console
$ docker pull caddy@sha256:d3e698bba2b53f43485241c9c8b87a48f34017f31adecf925fefd176d60b8422
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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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
$ docker pull caddy@sha256:2d25080ffc0c6a95bf450c4103c28eeda17d212c1b4e550fa5ecc3572c9d1c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6-builder` - linux; amd64

```console
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-alpine`

```console
$ docker pull caddy@sha256:c3f639c81b0fbb4b2d9d83345a6369dce5b90f3807c6f8474a2c2f2e3d5c969a
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
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:907bcf6ffbd9c87d579d9fd0c863633d3d5d3a4f7bbbe941849c977bcb479c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2.6-builder-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:2e8a4be822107da84510e9420e45153402e0561172b7d440cc58d9e42282e59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore`

```console
$ docker pull caddy@sha256:92e187efa2c1a4f653fe84781b9a61f067ecea93ec473084a2e54f46283c8db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6-windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3ebcc75c760fd3f09c9af3a083679243b86e38acac6b9c87d426f5e060bb5e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2.6-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8b07fddd6e884d7cd57b16fe8dfc8d764e50c606b804ace49eac539534eba9da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4`

```console
$ docker pull caddy@sha256:6b9c77b69da1cfdaa859416f1f6dc8f1af4c615e548bd7278956876134dc3244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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

### `caddy:2.6.4` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-alpine`

```console
$ docker pull caddy@sha256:d3e698bba2b53f43485241c9c8b87a48f34017f31adecf925fefd176d60b8422
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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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
$ docker pull caddy@sha256:2d25080ffc0c6a95bf450c4103c28eeda17d212c1b4e550fa5ecc3572c9d1c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6.4-builder` - linux; amd64

```console
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-alpine`

```console
$ docker pull caddy@sha256:c3f639c81b0fbb4b2d9d83345a6369dce5b90f3807c6f8474a2c2f2e3d5c969a
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
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:907bcf6ffbd9c87d579d9fd0c863633d3d5d3a4f7bbbe941849c977bcb479c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2.6.4-builder-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:2e8a4be822107da84510e9420e45153402e0561172b7d440cc58d9e42282e59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6.4-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore`

```console
$ docker pull caddy@sha256:92e187efa2c1a4f653fe84781b9a61f067ecea93ec473084a2e54f46283c8db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6.4-windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.6.4-windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-1809`

```console
$ docker pull caddy@sha256:3ebcc75c760fd3f09c9af3a083679243b86e38acac6b9c87d426f5e060bb5e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:2.6.4-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.4-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8b07fddd6e884d7cd57b16fe8dfc8d764e50c606b804ace49eac539534eba9da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:2.6.4-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:d3e698bba2b53f43485241c9c8b87a48f34017f31adecf925fefd176d60b8422
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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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
$ docker pull caddy@sha256:2d25080ffc0c6a95bf450c4103c28eeda17d212c1b4e550fa5ecc3572c9d1c5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:c3f639c81b0fbb4b2d9d83345a6369dce5b90f3807c6f8474a2c2f2e3d5c969a
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
$ docker pull caddy@sha256:daa80d7b1fddf55c852777a58e5c504bb0e51f24123cbec227b4344bf05f370d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.4 MB (131446561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66c494ede8be6ddc2e6283f577c23d1a6f46a623a61224ba08a49fbea2554c30`
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
# Wed, 29 Mar 2023 20:37:23 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 20:38:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 20:38:57 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 20:38:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 20:38:57 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 20:38:57 GMT
WORKDIR /go
# Thu, 30 Mar 2023 03:57:55 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 03:57:55 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 03:57:56 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 03:57:56 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 03:57:57 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 03:57:57 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 03:57:57 GMT
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
	-	`sha256:6c946529b76b434f0f1941a08bf919a4ab192201876972b0bc7c08556a3eec08`  
		Last Modified: Wed, 29 Mar 2023 20:42:23 GMT  
		Size: 122.4 MB (122369958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac7305c060e4a14280321acd25be5e41a2d90c2574eead251c882f436c084a`  
		Last Modified: Wed, 29 Mar 2023 20:42:07 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a94e8efdf1a08486c99d31332df5d1e66792808d9cef169d5f7da2ba31b7b08`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 4.2 MB (4198832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf32d4e5dc8a48ffdeb41bd0f9db6620d88a3c2473c7093b99caf8aff1c6f36`  
		Last Modified: Thu, 30 Mar 2023 03:58:11 GMT  
		Size: 1.2 MB (1217835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af895e9563f6c97810451cf4a1dd99c1d211aea36ade0fe844176ddc31fcb590`  
		Last Modified: Thu, 30 Mar 2023 03:58:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:c91da9e959da05b56111b8f4f666137d7d2092f6791c2f5719b1398b93be8ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127456652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1f540a8103e510ad77b7e2f9066f34966a821f3629e9bb1edcc25ddf2634f32`
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
# Wed, 29 Mar 2023 19:15:04 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 29 Mar 2023 19:16:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 29 Mar 2023 19:16:54 GMT
ENV GOPATH=/go
# Wed, 29 Mar 2023 19:16:54 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:16:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Wed, 29 Mar 2023 19:16:54 GMT
WORKDIR /go
# Thu, 30 Mar 2023 01:06:28 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 01:06:28 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 01:06:28 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 01:06:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 01:06:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 01:06:29 GMT
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
	-	`sha256:18a1fed17aac258fa8b4beeb6bec79beb2e4cec2374e88bc939dbf7d7de52a06`  
		Last Modified: Wed, 29 Mar 2023 19:21:57 GMT  
		Size: 118.7 MB (118732341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4493c55ec576e850675188d4dc34e2fc60e171fdbe3e702e05397d056a4c734`  
		Last Modified: Wed, 29 Mar 2023 19:21:38 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0190d9598e5c260f46e1fcb6b425de369a0fcef685bf8597d4c236e136d641b7`  
		Last Modified: Thu, 30 Mar 2023 01:06:43 GMT  
		Size: 4.2 MB (4160662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42700956bcf752d6a5fdbd375b8dfab9858673e184f08cf208827f344ff0a775`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 1.2 MB (1166070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33063a955244bbd19ff363b02019fcd6f1380e733bd0aa59ebe0be544551c628`  
		Last Modified: Thu, 30 Mar 2023 01:06:42 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:85d6e29f3060a4ed26710a47111d3a58f4ff7ae99f070671d7dfa8c5d4ec20c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126533688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ab5742763434c1d70c52df6a71aa6075ecfbd1b20e6203b628e59bed1c7ca82`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Thu, 02 Mar 2023 02:15:04 GMT
RUN apk add --no-cache ca-certificates
# Thu, 02 Mar 2023 02:15:04 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:02:58 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:04:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:04:43 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:04:44 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:00:21 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:00:21 GMT
WORKDIR /go
# Thu, 30 Mar 2023 00:39:46 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Thu, 30 Mar 2023 00:39:46 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 30 Mar 2023 00:39:46 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 30 Mar 2023 00:39:47 GMT
ENV XCADDY_SETCAP=1
# Thu, 30 Mar 2023 00:39:48 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 30 Mar 2023 00:39:48 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 30 Mar 2023 00:39:48 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4962ca8504034f69427a90f2b07cfde1e4c20297e4507d5620bb7ea27e646919`  
		Last Modified: Thu, 02 Mar 2023 02:26:02 GMT  
		Size: 285.4 KB (285445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4036193e5613622435e9aad6484115a921a92fa95ac49886a5aed81e6bfc5e02`  
		Last Modified: Wed, 08 Mar 2023 00:11:37 GMT  
		Size: 118.5 MB (118486599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aebc73a2c5c2ce7aa70f6b809e9aebc8bc0237a6e891eb2d3175567fd52e695`  
		Last Modified: Mon, 27 Mar 2023 22:01:49 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0199e88399fe3799d9bc09ea1ba4b32265aa08523047d4225489df464638bf1`  
		Last Modified: Thu, 30 Mar 2023 00:40:20 GMT  
		Size: 3.7 MB (3729258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d2c7664417c613cdb3c8b535151b74eda789e83de11a4db895c21b4fd7a59d7`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 1.2 MB (1163330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70fe679b05aabbe72f9ba94c90109a46775a2c2fd76a40da48cd100ae51473f`  
		Last Modified: Thu, 30 Mar 2023 00:40:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:88e29b725bfdf4697bcc2625ba36c741d1df8b07a2318067391c1a4e85d1c448
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.8 MB (125849857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f20a960799a322bef771a3074b0bbcb9a773dbdf204fd352e985c270daf4ba42`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:38:33 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:38:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:43:17 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:44:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:44:26 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:44:26 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:45:29 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:45:29 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:50 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:50 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:50 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55522c79112429742fe76c795b9509c5cd1e8198e0caa2a1e355c0e60a719576`  
		Last Modified: Fri, 10 Feb 2023 22:44:19 GMT  
		Size: 286.3 KB (286257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1815dcbf43e87e122cc76a24663b7c0d6e01ad03c3be30a7dc13c1bf941c595`  
		Last Modified: Tue, 07 Mar 2023 23:49:19 GMT  
		Size: 116.9 MB (116933985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492bf1cda8a3b74dd16750138f89f25a8fabb107d8ab44a4ee9a47c662fe0fce`  
		Last Modified: Mon, 27 Mar 2023 22:46:49 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f513cda03f9ce4503c9d7437df5d97b5505277b035936cdcff206f31aff4c0`  
		Last Modified: Tue, 28 Mar 2023 02:21:04 GMT  
		Size: 4.2 MB (4243361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6641b95880af38fe5617f1d844a69addfbcd13f4f0d025cab37dbefb42d6dc`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 1.1 MB (1123734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889b135a05b02051d99577ae21ac82cb696a51e8b3388e676fd771a0c409b83b`  
		Last Modified: Tue, 28 Mar 2023 02:21:03 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:158a71268e5dadc7a17ece59757fa75c007c48d89431d52ec0a75fa786ad4a39
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.6 MB (126600083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36a1d171f016e8001d702174e9d6ae692acd08f96b872b16dc8d5f0cf33decdf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:40:13 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:40:14 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 08 Mar 2023 00:23:54 GMT
ENV GOLANG_VERSION=1.19.7
# Wed, 08 Mar 2023 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 08 Mar 2023 00:26:35 GMT
ENV GOPATH=/go
# Wed, 08 Mar 2023 00:26:35 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:22:25 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:22:25 GMT
WORKDIR /go
# Tue, 28 Mar 2023 02:20:01 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 02:20:01 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 02:20:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 02:20:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 02:20:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 02:20:04 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 02:20:04 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:788962e1689dbb14c760601cbf633ae350e98e3a045f8010924cd585de6b6a3e`  
		Last Modified: Fri, 10 Feb 2023 22:53:32 GMT  
		Size: 286.6 KB (286645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ba367c1dc6d801c3405d9bb1162f99efd64face4f7fd7d5f97d1cac94ffc831`  
		Last Modified: Wed, 08 Mar 2023 00:34:09 GMT  
		Size: 117.3 MB (117328058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d445a3c38cb5cab10d0efbdd63a96f5b31e7e971e8bd0c78e91a49254800ec09`  
		Last Modified: Mon, 27 Mar 2023 22:23:44 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35310466c8605858dcf0946bef5e0ea4dd7fd048b483fa6023c3f7028b88d831`  
		Last Modified: Tue, 28 Mar 2023 02:20:21 GMT  
		Size: 4.5 MB (4488181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b7f7261e104b3cbfe429c5454674f7878dccbfbb0f177fb410a316794c7c4a1`  
		Last Modified: Tue, 28 Mar 2023 02:20:20 GMT  
		Size: 1.1 MB (1105889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9660e926fac3a8bd7361df5b2ef8a1ced0a398a632df1896eea8d5018c8ee89d`  
		Last Modified: Tue, 28 Mar 2023 02:20:19 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:c60cbc54f7f31e01ab91e230ea605a662b51aa7adb93b90c5db7b48f894ddf1b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.6 MB (129610920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6594269645b9139ea18ee89794c843d8633d742e808d7baf5e7f188f76f9c472`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:27:44 GMT
RUN apk add --no-cache ca-certificates
# Fri, 10 Feb 2023 22:27:44 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 07 Mar 2023 23:47:03 GMT
ENV GOLANG_VERSION=1.19.7
# Tue, 07 Mar 2023 23:48:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.19.7.src.tar.gz'; 		sha256='775bdf285ceaba940da8a2fe20122500efd7a0b65dbcee85247854a8d7402633'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			if [ "${GOARCH:-}" = '386' ]; then 				export CGO_CFLAGS='-fno-stack-protector'; 			fi; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 07 Mar 2023 23:48:53 GMT
ENV GOPATH=/go
# Tue, 07 Mar 2023 23:48:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 27 Mar 2023 22:43:39 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 1777 "$GOPATH"
# Mon, 27 Mar 2023 22:43:39 GMT
WORKDIR /go
# Tue, 28 Mar 2023 00:54:02 GMT
RUN apk add --no-cache 	ca-certificates 	git 	libcap
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_VERSION=v0.3.2
# Tue, 28 Mar 2023 00:54:02 GMT
ENV CADDY_VERSION=v2.6.4
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 28 Mar 2023 00:54:02 GMT
ENV XCADDY_SETCAP=1
# Tue, 28 Mar 2023 00:54:03 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='2538d080f065cf1c5a41c9c14dd6acd55783e004c7ea3fdd6e1bc07c4d846a85b78d5de1111391fda71d48cad9d542a0741593e5b25ea9826faaee74577d8a98' ;; 		armhf)   binArch='armv6'; checksum='5bd99dfc28d867253275c2a6753425a1e8445385449cd5414c8bb14fdf7b513f468c69e0ae8ba431cf4b5e2b5f77666dda2a6811fbe8a1718cae377387319b36' ;; 		armv7)   binArch='armv7'; checksum='e8ea697bcbe029c81ce183b5ec44d095d8919f62a7170a0697dd7531d5a87c980b9aac1442638bf4dee1e60abe0ad698dfa56bed222fe9329ff274f5973f12fe' ;; 		aarch64) binArch='arm64'; checksum='afbf26528c4238a7d6eaa375c1367d213f7d3359e97193b996a896b89fb852531d33581b8cef6432bd866d1488f5f98ed43a198732c45d5b9d008eb9316d36ab' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='519e8d7575507e49ddd7d58d168c6223802b94a8954284956db4b72133bf3027de03f9bfc0dc578373ebcb49d668a140fcd54d90888c17cdbbef6ab182a8b511' ;; 		s390x)   binArch='s390x'; checksum='b95078a4231acd54bd56c70d110709c9e290089200855c9448259621c983fa5ecfa925a1e6ab59459750bc6abb936422433543b6079fa547dea4dc08d5daabf9' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 28 Mar 2023 00:54:03 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 28 Mar 2023 00:54:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa53ed2f1b70a83e3a15cae881ca47cd40f6ac11060717cdbbd4e405f9d586`  
		Last Modified: Fri, 10 Feb 2023 22:37:18 GMT  
		Size: 285.0 KB (285032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d83de48b90cbc8ae74a05d0af343e28f82727b9797b0b45ed9a70fa837a9a5`  
		Last Modified: Tue, 07 Mar 2023 23:53:54 GMT  
		Size: 120.8 MB (120808046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a59eb753e2606c1d0205a55c33b7492320e988338a4cd3bacf6657cfefb7be22`  
		Last Modified: Mon, 27 Mar 2023 22:44:35 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3d4631dcb7ef1f957f6674cdc65f37660b677f34441e1c25592b06546fb769`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 4.2 MB (4171767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11a69ab3bd5e3b23bd9234f41b3350176a59ae1a4f4cc07136a58d415414af8`  
		Last Modified: Tue, 28 Mar 2023 00:54:22 GMT  
		Size: 1.2 MB (1170398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f79a8c2fcdf8b9f383f9b6947cf64c012a7a41ab9321f7e3782081abdc5a0b`  
		Last Modified: Tue, 28 Mar 2023 00:54:21 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:907bcf6ffbd9c87d579d9fd0c863633d3d5d3a4f7bbbe941849c977bcb479c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c9032910fbe59986e17e53ecbfd5ea3e2881f9620a93059d210565e8b59a25ec
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2198807920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bb35fb2c0019120cb2f52989b07f2edcb7025e0f2c94730d2072d883a96d0e8`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:05:31 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:05:32 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:05:33 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:05:34 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:08:43 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:08:45 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:11:00 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:30:04 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:35:29 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:42:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:42:32 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:42:32 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:42:33 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:43:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:43:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96cd8204a3a0f91264f1d80a1823c6302144beba7b949672383f79a4b0eaaaaa`  
		Last Modified: Thu, 16 Mar 2023 02:46:22 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f9b5c8cc42aa4e27c584910b32e3dd61b08d3737c3a4bd57c718c6bdf4e918c`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d294e5fa55a2c856286550cda7d5754988031614630a73de68e7a91bb9780b1d`  
		Last Modified: Thu, 16 Mar 2023 02:46:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ae3806c822a2819e77add7db0ffb98fbf5a4db7f6b546da7836b3c5e280921`  
		Last Modified: Thu, 16 Mar 2023 02:46:18 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8496692041c620f4a5d6248542d1fbbe277a127d0c8f999f8ee24e4dd245495c`  
		Last Modified: Thu, 16 Mar 2023 02:46:27 GMT  
		Size: 25.6 MB (25579220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a76c28450756e3ff6ea6233e7b9cf00fb53673383e2b7ca14eebe7e99e29d8`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846ce11a3cbfe6ecdd0116b5beb678a12cfc66ead578bf96aef94c527e0eb3ed`  
		Last Modified: Thu, 16 Mar 2023 02:46:16 GMT  
		Size: 323.2 KB (323191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007aa50ce0d4dfd36bfd2d18608fce2ef6a37354603df606438b96a07124bc0f`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f5c1dcb53aa73aada7ad9d4b1bb9dc43535afd2526802db572757a4f3b1525`  
		Last Modified: Thu, 16 Mar 2023 02:50:48 GMT  
		Size: 157.8 MB (157764104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1316d76362a1808f7b882074ea5cbed1cce2892caa37cb311f38a73fdea9dcda`  
		Last Modified: Thu, 16 Mar 2023 02:50:00 GMT  
		Size: 1.5 KB (1524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c91cd00a563121fa30dbc382f5027a18ebf90cc2754e79980f37c8685c7030`  
		Last Modified: Thu, 16 Mar 2023 04:46:26 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e9290bf0d4bfd4af381743a93f904c36159f0bb345e98226221093c2adb10c`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:202bbf38db2cbd0d97b70aab758abe41b4bdf86de6bbf6920ef866d23309fcb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02200a8e9b0587ea6d794a97d1478b24edc0552d50eb20ae08021c5946e976f3`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8895a312263f89855cc0e57b315b57ccef5c314eb6637732ffe3beb42297cd2`  
		Last Modified: Thu, 16 Mar 2023 04:46:25 GMT  
		Size: 1.6 MB (1614512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fcd18dab8ce707123ce4789697f284017a7694305fed4996c6cdcff9019cba`  
		Last Modified: Thu, 16 Mar 2023 04:46:24 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:2e8a4be822107da84510e9420e45153402e0561172b7d440cc58d9e42282e59d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:43755617b9c9e24b290317d14a47924021fe4560c06ffefed4deaa4bb2634439
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.9 GB (1900128993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409c3b26aa7f8acdf03c6147aef127176c4ac57d987e8696393154196c8a5e3b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 02:00:02 GMT
ENV GIT_VERSION=2.23.0
# Thu, 16 Mar 2023 02:00:03 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 16 Mar 2023 02:00:04 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 16 Mar 2023 02:00:05 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 16 Mar 2023 02:00:58 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:01:00 GMT
ENV GOPATH=C:\go
# Thu, 16 Mar 2023 02:01:33 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 16 Mar 2023 02:25:32 GMT
ENV GOLANG_VERSION=1.19.7
# Thu, 16 Mar 2023 02:29:52 GMT
RUN $url = 'https://dl.google.com/go/go1.19.7.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '2fd57332bc55f6d8c4860afa22301d0a2439ad63ba91e3d96b69c03c824df217'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Thu, 16 Mar 2023 02:29:54 GMT
WORKDIR C:\go
# Thu, 16 Mar 2023 04:44:00 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:44:01 GMT
ENV XCADDY_VERSION=v0.3.2
# Thu, 16 Mar 2023 04:44:02 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:44:03 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 16 Mar 2023 04:44:48 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.2/xcaddy_0.3.2_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('8de1cb65e555e8d7f1124d384904cd53a37d1914106af6ec1cef92f1975bd66b5a1f0e066c2c6b68c85d67de54d52f170f539dff117ce97f4166d8e984a728ba')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Thu, 16 Mar 2023 04:44:49 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc92251be4a3030d0c1ad240813d13619cab05ed6114271f4f31e2e37ade28a`  
		Last Modified: Thu, 16 Mar 2023 02:45:31 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a39cf6573a7f6e725c805ddf277348509d33f67f8a6216a2a0e1b04f1be37158`  
		Last Modified: Thu, 16 Mar 2023 02:45:26 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db9d107c8208ad44d6a6873db70ff7887d6d3afad4cf934a0b2babd2cc48ca`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4f39a3aa63487027366004c347541623d246d80d6fe57e23ce4040c94709ef`  
		Last Modified: Thu, 16 Mar 2023 02:45:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3be7e7a27e770912dcb9b9a3ef7e82764a250d64726013c23ac515b5b810573`  
		Last Modified: Thu, 16 Mar 2023 02:45:35 GMT  
		Size: 25.8 MB (25825670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5990e3c132a38a31cb5f36c7fe62af4390ed95711decdc15695ce969dbfc38`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2807b4fd79ee2ec379a6f147d376f4c869daabbd081cb9dbb601ec6d397dd92`  
		Last Modified: Thu, 16 Mar 2023 02:45:23 GMT  
		Size: 540.0 KB (540000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad790a3851130adf4c71fc7d72412ab2f7dbf7fac4c6db61810a97ed9481eac`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4447d8d3267fc37e218d5e97a18e5aca96cf41db6b63c88f72121959335b001b`  
		Last Modified: Thu, 16 Mar 2023 02:49:51 GMT  
		Size: 158.0 MB (157968511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f97e3d123edfa2467d66ae71fecb73cac296fafb9313779a7a866020f5b8811`  
		Last Modified: Thu, 16 Mar 2023 02:48:55 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ade9ec32648c51fcb44fd7c4278fb07c380739eb348a726bc1c4d15f3fb9c18`  
		Last Modified: Thu, 16 Mar 2023 04:46:45 GMT  
		Size: 1.4 KB (1365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbea3f2cb965aece9d2a8734bc18988a58d7496a02fe295d7f64613f102e96d`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4667b8c2fe9609bfe04bd21e55cadce07b92a28077e6bda07b8f1560523785e0`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef28e7dee29b79ab6bcf588fea449d79267bf66b12d47d47d5f9e5dcd80e3e8`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbd1898d180fe7d68b7a3e64e85ea504104f506e62f6cd5a8c01087d645cf77`  
		Last Modified: Thu, 16 Mar 2023 04:46:44 GMT  
		Size: 1.8 MB (1836501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a814a6af127f80e0527e5154302f49d5513b7155a3ead8c65f8bb613ece4ad`  
		Last Modified: Thu, 16 Mar 2023 04:46:43 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:6b9c77b69da1cfdaa859416f1f6dc8f1af4c615e548bd7278956876134dc3244
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

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
$ docker pull caddy@sha256:8861ab3ae3d0c180e38142c2f7482f9ce1773419eb29ed9d6d18308246858093
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.0 MB (15955172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5819f0ab4928a30c29293a27299a3b44371cd3bd97df91432ef7b3f43b692d8c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:13:21 GMT
RUN apk add --no-cache 	ca-certificates 	libcap 	mailcap
# Fri, 10 Feb 2023 22:13:23 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"
# Wed, 15 Feb 2023 19:16:26 GMT
ENV CADDY_VERSION=v2.6.4
# Wed, 15 Feb 2023 19:16:40 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='eed413b035ffacedfaf751a8431285c5d9a0a81a2a861444f4b95dd4c7508eabe2f3fcba6c5b8e6c70e30c9351dfa96ba39def47fa0879334d965dae3a869f1a' ;; 		armhf)   binArch='armv6'; checksum='72ab7c0bd627415cafcf3cc1adebdff0dcb2bb8f81e8969da356f741ae91289c231e20b29dbe268d501f252402adde151dcf7f3acfaf886c0b2dc02143fe5c01' ;; 		armv7)   binArch='armv7'; checksum='de8cb9cfb7d81e822d06ab55059d76dd285ed6d9b2861cd7ee5334622cf5938c61e0f0efcc4c6ccff0847b1c485752c670aa8d672fce5ca36edfd9c0714dc40c' ;; 		aarch64) binArch='arm64'; checksum='6513d40365c0570ff72c751db2d5f898d4ee9abe9241e73c3ad1062e21128745071b4efd3cc3443fc04fae2da49b69f06f70aadbe79d6a5327cc677fb86fb982' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='0341763653017b530a7b0137b6d1296101b21bec7a81b6320ed70479c342dc671d8a538dc07913b9b834e798b95097b4d9190986a296eed7f1a612bfa33fd752' ;; 		s390x)   binArch='s390x'; checksum='3d9779898401cbf37c3e5f1cfdbe253739340f2446d464e421db063c674e6a0ca355ae3c2a8374454ef470eed13f17493b40d259d3073775843bd5a1e47a7dc6' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	setcap cap_net_bind_service=+ep /usr/bin/caddy; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 15 Feb 2023 19:16:41 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 15 Feb 2023 19:16:42 GMT
ENV XDG_DATA_HOME=/data
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Wed, 15 Feb 2023 19:16:42 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 15 Feb 2023 19:16:43 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 15 Feb 2023 19:16:44 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 15 Feb 2023 19:16:45 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 80
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443
# Wed, 15 Feb 2023 19:16:46 GMT
EXPOSE 443/udp
# Wed, 15 Feb 2023 19:16:47 GMT
EXPOSE 2019
# Wed, 15 Feb 2023 19:16:47 GMT
WORKDIR /srv
# Wed, 15 Feb 2023 19:16:48 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782bd0321e6539bb7dac8574fd36bad22059ef06bb63dc842165f69d0a821572`  
		Last Modified: Fri, 10 Feb 2023 22:14:16 GMT  
		Size: 363.1 KB (363088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb806b2600b0209a73fc7175ab778d0224661034b2f722bd1a0aec1eb9eabe3d`  
		Last Modified: Fri, 10 Feb 2023 22:14:15 GMT  
		Size: 7.6 KB (7558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd7c8ae860931dd79dea76d33bc21bb11d89cd4d133cdb41078b040afc6633e`  
		Last Modified: Wed, 15 Feb 2023 19:17:41 GMT  
		Size: 12.8 MB (12779898 bytes)  
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

### `caddy:latest` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:92e187efa2c1a4f653fe84781b9a61f067ecea93ec473084a2e54f46283c8db3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.4131; amd64
	-	windows version 10.0.20348.1607; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:3ebcc75c760fd3f09c9af3a083679243b86e38acac6b9c87d426f5e060bb5e3e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4131; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.4131; amd64

```console
$ docker pull caddy@sha256:c3553096a5433b6fbe792341807e3f32eab84b2ddb131e5692ed9f48d61f9238
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2028971522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f30781ff32bdeaa628f432969c3777c7f08d0cb8ccd0aa729ddcb79f384081`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Sat, 11 Mar 2023 10:37:22 GMT
RUN Install update 10.0.17763.4131
# Thu, 16 Mar 2023 00:41:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:37:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:37:15 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:38:46 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:38:47 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:38:48 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:38:49 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:38:50 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:38:51 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:38:52 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:38:53 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:38:54 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:38:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:38:56 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:38:57 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:38:58 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:38:59 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:39:00 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:40:02 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:40:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a92048040b3b13af10f8287baabaddbb2759dfc77b1fb43f89b38b3275467f93`  
		Last Modified: Thu, 16 Mar 2023 01:42:29 GMT  
		Size: 305.6 MB (305565048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8e4e0836091bdd33e8adb56d1e13b8096550727a20534e2a2ab9298c86fa09`  
		Last Modified: Thu, 16 Mar 2023 01:41:16 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:477ecc5db1131881af63bb70c5decf4d970469b1dfb97b7f1b66d78a3a4ced23`  
		Last Modified: Thu, 16 Mar 2023 04:45:39 GMT  
		Size: 492.8 KB (492825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b723ad454b8fb718a2091f7f97219cdbfd1f499eddb2ecbf5d516325747f3f17`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc31dbad1d85cecfaf38780eb2b4df4af2ece2c2e66814fe9c91e4b22262d64`  
		Last Modified: Thu, 16 Mar 2023 04:45:43 GMT  
		Size: 14.7 MB (14657569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e7896625898f0fa4de76d6293ba2559c3cac0f1bbba978db77949337e46327`  
		Last Modified: Thu, 16 Mar 2023 04:45:38 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:679a0290b4f1fbeb35bb3ab602f42e40f08aad589efe947754c6eebb61042e3a`  
		Last Modified: Thu, 16 Mar 2023 04:45:37 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b163264b38bcaf56ee78cf3785febadf11e8e4093438bac30e7ba928d7538985`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634bbc14b065b600a90e2fd073f647d01a5b2493e2929b96a96f8cabbbcffe7`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97bcb880f6e1a8c5b3a2031606c24a2276622686219d8f837c3856000c759379`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe23ba8107a87636d0fefe0e244d3d78b1a5dad337826ff2ab2c7999596a563`  
		Last Modified: Thu, 16 Mar 2023 04:45:36 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db25f9b545fac2c61bcd08c0a9328128838c9dda628744a3fc3ee1d0ce64d06`  
		Last Modified: Thu, 16 Mar 2023 04:45:35 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e256a3d6e90e60b1605b49756254acddbd784c6875e50573d7584e98374871a4`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe4191792d436a22e5cf97b56c891aa895ab08ca1ef166efdaf7dbbcc7f451b`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce796488ba8f9f5b8c8ebb451f1913c5abde57233cefec2270a63010a271f99`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7fae93b5360cc0dd5e7535a1d9d284e89f0e2271e8d5544b516db8b56212ac`  
		Last Modified: Thu, 16 Mar 2023 04:45:34 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bcf1464c6baaf3f6d4157cfc582120b71cd016a44f06c872c160c12b6f38db`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6187e7671fbd81e2732f7366a17b654e64e6b934acf60d904ca32b1b6bc3261e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21b4ed923e5be42f36152cd750efc2c9cc9160935dd4b9cc874a7b5826e56124`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54acced296ffcaa79a329f25fac77865507005ba57a3a791ec0a2818e5ba56d8`  
		Last Modified: Thu, 16 Mar 2023 04:45:33 GMT  
		Size: 290.0 KB (289995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd90ad1f757c0d8fc2e1110a6e06bbf3a3768e4ba59789adaf56fc51a781865e`  
		Last Modified: Thu, 16 Mar 2023 04:45:32 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:8b07fddd6e884d7cd57b16fe8dfc8d764e50c606b804ace49eac539534eba9da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1607; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.1607; amd64

```console
$ docker pull caddy@sha256:ff00e9f1aff43bd762743459cd3b864ee474185aa61944a7bf96317269ed1bac
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1729934812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d95c20254ee986634359a888974724ea0631d7084a514b14ddfa5b1e8173afcb`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Fri, 10 Mar 2023 06:37:36 GMT
RUN Install update 10.0.20348.1607
# Thu, 16 Mar 2023 00:38:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 16 Mar 2023 04:40:57 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/305fe484cc8a9ac72900e8cc172d652102a87240/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Thu, 16 Mar 2023 04:40:58 GMT
ENV CADDY_VERSION=v2.6.4
# Thu, 16 Mar 2023 04:41:30 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.6.4/caddy_2.6.4_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('e2a9a708786cc498cf4b12c0aaf2c9731cc89ccef71a7da4c2be60e18d730675890c2d6bbddd3d8347e5f89f348d5e74fbfbf339ed1ec280f5caf69c3849a243')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Thu, 16 Mar 2023 04:41:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Thu, 16 Mar 2023 04:41:37 GMT
ENV XDG_DATA_HOME=c:/data
# Thu, 16 Mar 2023 04:41:39 GMT
LABEL org.opencontainers.image.version=v2.6.4
# Thu, 16 Mar 2023 04:41:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 16 Mar 2023 04:41:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 16 Mar 2023 04:41:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 16 Mar 2023 04:41:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 16 Mar 2023 04:41:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 16 Mar 2023 04:41:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 16 Mar 2023 04:41:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 16 Mar 2023 04:41:47 GMT
EXPOSE 80
# Thu, 16 Mar 2023 04:41:48 GMT
EXPOSE 443
# Thu, 16 Mar 2023 04:41:49 GMT
EXPOSE 443/udp
# Thu, 16 Mar 2023 04:41:50 GMT
EXPOSE 2019
# Thu, 16 Mar 2023 04:42:16 GMT
RUN caddy version
# Thu, 16 Mar 2023 04:42:17 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c921d7eac594f5e3ce3ef10adb8fd0f71bdbb713c4854336b995d25f89c44d42`  
		Last Modified: Thu, 16 Mar 2023 01:41:04 GMT  
		Size: 327.9 MB (327911088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca4593035ae0e8d1b6e6eb1b053fddc6a6824b28f45f99de726d752d2c0f72`  
		Last Modified: Thu, 16 Mar 2023 01:39:50 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63a518108c0512b176391a57676def0a7d9cad2621d9075f7e446fa52065fb4`  
		Last Modified: Thu, 16 Mar 2023 04:46:06 GMT  
		Size: 746.0 KB (746007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c0bbba28efc2176e9aa30a5a294c086bc887a26892e9730a5f8a2cad67ea0b`  
		Last Modified: Thu, 16 Mar 2023 04:46:05 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3051382aee23f9dab9e33db29e5f4bc6bd76731cb7b3fd6ffc81babfdabc0bcb`  
		Last Modified: Thu, 16 Mar 2023 04:46:09 GMT  
		Size: 14.9 MB (14879237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e5a88bf4691b6b4c1a078a21b305be9a033545120d493ba4337fd9f7d994d4`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac6906695247907de09c83e0098ec67aa06edd8a74d2b4a4a308c721dd50533`  
		Last Modified: Thu, 16 Mar 2023 04:46:04 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb79e610a8de5b904ff29c193541dc397c6ea147d05e2a731c985dd565f5b83`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8056d626699bdae01adb2eac08605cb8288847a63091852dd14b833bf887b2f1`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.4 KB (1354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f942776b9ba01a39cb71e00c37db5dead27ad4d07719bf9141136f796cd3dff9`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc0eb0399c2afb264984b262c133150825b97f71beb1f48197ad5fd9bf09925`  
		Last Modified: Thu, 16 Mar 2023 04:46:03 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdeb580c2d61276e3c0620fe105c0a23f0ce0a97b4c2479055ec7fba6f7641b4`  
		Last Modified: Thu, 16 Mar 2023 04:46:02 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fcaffc984375a548b86d400397faa3d6bdc8c7db365f065eff5a9b0d11bbb7`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f69d7316137bc20a03e7905e68701ba7869f532fa99bfef9de55248338094f06`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95309000e17eea50844aef16fe07499842a7fef86bcc95bc72b7824bae001110`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0082ee2f7eedf75ec4bc67db82c1722b0c3bceafd23f57ad5558ab024a09249`  
		Last Modified: Thu, 16 Mar 2023 04:46:01 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d628eee6e0e340f6fdc6f888f1b94bb8bfc088bbc4f2fc0fe731ff9313425d4`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab513c46a22e0448aa4c504b4c0795a5cc3440d8192fef1d064dc87931af7b14`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116b5fac64ee319780d2ebf62c59f34c4dc25ceb93c6692a3aef1620d01f0c19`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0cbd8ae522ae0b19628239d4ae6f5b70aac9db799def76530068ae7f11258a`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 347.0 KB (346955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c699819df78f8c46f2092090f7b43fa00667802c7853a0ae56e8dc2e32f6b5`  
		Last Modified: Thu, 16 Mar 2023 04:45:59 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
