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
-	[`caddy:2.5.2`](#caddy252)
-	[`caddy:2.5.2-alpine`](#caddy252-alpine)
-	[`caddy:2.5.2-builder`](#caddy252-builder)
-	[`caddy:2.5.2-builder-alpine`](#caddy252-builder-alpine)
-	[`caddy:2.5.2-builder-windowsservercore-1809`](#caddy252-builder-windowsservercore-1809)
-	[`caddy:2.5.2-builder-windowsservercore-ltsc2022`](#caddy252-builder-windowsservercore-ltsc2022)
-	[`caddy:2.5.2-windowsservercore`](#caddy252-windowsservercore)
-	[`caddy:2.5.2-windowsservercore-1809`](#caddy252-windowsservercore-1809)
-	[`caddy:2.5.2-windowsservercore-ltsc2022`](#caddy252-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:7faf730343c6bd50150b13b73bac1f97886a30ae15f145e5d301c8299949bb52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:203756314ab8a08842b738edf048a49eda65caadbaa67d9efb961f6b64d48286
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
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:1a5b266bad59ada954eabcfdf6a0d3dfdd005e71d4e37523aec4d9dbd3d69cd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:f646f2da87592fea82147f9c42377301884df47d42bbca5016da95010d85044c
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
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:61656a3c4dc45283179800b954655f7fdb6e593ea84c2dd21a57f509a897a1cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:97856175998bb682fc518bdfaa61ab1eb23d732ceff5b1d5afa9d4e22dafc379
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:a6506a1cb644e10461e5a43a0514aef50d49a62d898aa73e9c3604ecfc697cb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:744553df106b3067f1d20b1b0c6431c3b6fa66c99b0fabe0cd9518beecbad6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:4b56a1d12cc2f346deceebca9dca6640d81a1ca369c68151f5dd2d9c3ffccbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2`

```console
$ docker pull caddy@sha256:7faf730343c6bd50150b13b73bac1f97886a30ae15f145e5d301c8299949bb52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2` - linux; amd64

```console
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-alpine`

```console
$ docker pull caddy@sha256:203756314ab8a08842b738edf048a49eda65caadbaa67d9efb961f6b64d48286
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.2-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder`

```console
$ docker pull caddy@sha256:1a5b266bad59ada954eabcfdf6a0d3dfdd005e71d4e37523aec4d9dbd3d69cd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-alpine`

```console
$ docker pull caddy@sha256:f646f2da87592fea82147f9c42377301884df47d42bbca5016da95010d85044c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `caddy:2.5.2-builder-alpine` - linux; amd64

```console
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:61656a3c4dc45283179800b954655f7fdb6e593ea84c2dd21a57f509a897a1cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2.5.2-builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:97856175998bb682fc518bdfaa61ab1eb23d732ceff5b1d5afa9d4e22dafc379
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore`

```console
$ docker pull caddy@sha256:a6506a1cb644e10461e5a43a0514aef50d49a62d898aa73e9c3604ecfc697cb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2-windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:744553df106b3067f1d20b1b0c6431c3b6fa66c99b0fabe0cd9518beecbad6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2.5.2-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:4b56a1d12cc2f346deceebca9dca6640d81a1ca369c68151f5dd2d9c3ffccbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:2.5.2-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:alpine`

```console
$ docker pull caddy@sha256:203756314ab8a08842b738edf048a49eda65caadbaa67d9efb961f6b64d48286
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
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:1a5b266bad59ada954eabcfdf6a0d3dfdd005e71d4e37523aec4d9dbd3d69cd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:f646f2da87592fea82147f9c42377301884df47d42bbca5016da95010d85044c
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
$ docker pull caddy@sha256:2458fd7c8ccf7d56c01b51960839f9073bb3cfceada41814d6041b30f135443a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126545048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7e0fe9c201348c7e90424f862a847f30be610248d7acba0403ba06676d43ef9`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:56:26 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:56:26 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:56:27 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:58:25 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:00:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:00:07 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:00:07 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:00:07 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:00:08 GMT
WORKDIR /go
# Tue, 19 Jul 2022 00:21:13 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 00:21:14 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:14 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 00:21:16 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 00:21:16 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 00:21:16 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d450d4da0343091dd049727bcf8ccaae8c22b9b11cbb26823c403343ca9faa1c`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 271.8 KB (271834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8162171ecb65551f90de8eb79be7a98850c0b4fa7af6e31150ad932d3ea3fb32`  
		Last Modified: Mon, 18 Jul 2022 23:02:52 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06619bbbb66c1a62f1daf795edf69bf6f9edd45d40385499ddf3c8933e2970fa`  
		Last Modified: Mon, 18 Jul 2022 23:03:44 GMT  
		Size: 115.2 MB (115243244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ae7f56e770e473524f005ecc856e76c7006bc50f458cd7f4f4839a30ffd8503`  
		Last Modified: Mon, 18 Jul 2022 23:03:27 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe0de796bcdbca22ef971ca9379652b73fe6f6611044d8c5a13920c2c85f7ac`  
		Last Modified: Tue, 19 Jul 2022 00:21:49 GMT  
		Size: 6.9 MB (6941041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eefe7ffaa8d8c49248bd055633d2e4f402ae6902fb07634f47d589963a22e0`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449e49aa7fa01019e872016f4fbdcdf1d166c5984e6ed7e2493e0c072bf45b72`  
		Last Modified: Tue, 19 Jul 2022 00:21:48 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:17a939439945ed3695150556252a1fec218fda205bb61fffa92f0e63a60b724c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.6 MB (122574642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f2c8b91d3c0d5787149d6241d2a3c4ed6f891eee00960eb2b982020ed8c484cd`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:25:28 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 20:25:30 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:25:30 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:30:01 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 20:33:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 20:33:56 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 20:33:57 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 20:33:58 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 20:33:58 GMT
WORKDIR /go
# Tue, 19 Jul 2022 04:30:47 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 04:30:47 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 04:30:48 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 04:30:48 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 04:30:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 04:30:51 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 04:30:51 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f1dfbc0803401d6a3a9b0e394f0f8747493f1b55833610c10353b62101021d4`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 272.0 KB (272036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa1f1aae2b5f322638c7c3459c306aec10d9a9d017ae9df2a4abaea105e427aa`  
		Last Modified: Mon, 18 Jul 2022 20:39:59 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222ee8162b753fe070212870b3f4014463f1c6c1e5038013ba3d465af82c91db`  
		Last Modified: Mon, 18 Jul 2022 20:42:55 GMT  
		Size: 111.7 MB (111658413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cba8b54c57dba63af350aeebb27aeb03f8f1e68ee0275ceeef446e8c16f791`  
		Last Modified: Mon, 18 Jul 2022 20:41:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdbcacf7e8f2acf43e24de754f732e0cda1d8d20bf1a2c80683944849fb11a4b`  
		Last Modified: Tue, 19 Jul 2022 04:32:00 GMT  
		Size: 6.8 MB (6807887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b613faf0b6fea50ce5e8d80810d39c21300029da63efa7cec970b5d1227c32`  
		Last Modified: Tue, 19 Jul 2022 04:31:57 GMT  
		Size: 1.2 MB (1229161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d3e1f3d942ecf99ed46e1b9e8bb7a7a5c0ce0652ebc376312c72230ae94450`  
		Last Modified: Tue, 19 Jul 2022 04:31:56 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:b9932476c39e20095ff7398bd8eaf554a341720f51699f68dab80060b20cc4bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121401716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2e81ae20af980ea0be616e2bad4c39b711ac8e035ff9cff2a7adeedd620a15`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 23:04:00 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 23:04:01 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 23:04:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:08:50 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 23:12:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 23:12:40 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 23:12:40 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 23:12:42 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 23:12:42 GMT
WORKDIR /go
# Tue, 19 Jul 2022 11:58:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 11:58:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 11:58:02 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 11:58:02 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 11:58:04 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 11:58:05 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 11:58:05 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310150171570b715e2477d77efca60a48d1ddbc81587d89c7cbc2460c1ed361`  
		Last Modified: Mon, 18 Jul 2022 23:20:36 GMT  
		Size: 271.0 KB (270981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb9d181ccdc5fbe5ffe9c2f289c1c6956e03074fdc6d8a2d146e1fa5000906c4`  
		Last Modified: Mon, 18 Jul 2022 23:20:35 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f2170480b981d82e41321069f388412642869fed23f3bb70cd2758050cc4eb`  
		Last Modified: Mon, 18 Jul 2022 23:23:28 GMT  
		Size: 111.4 MB (111422389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7ef2dcb31da3f2386f54994ad80e629f36fdad88a3b8fbc126d62630df370f`  
		Last Modified: Mon, 18 Jul 2022 23:22:28 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811feb3a9759a22d36c960e3270bb8507f56e562a3a6a126ade78cdeb6f1ca3`  
		Last Modified: Tue, 19 Jul 2022 11:59:13 GMT  
		Size: 6.1 MB (6067310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eca07f2ebd4c86412c9d753b2971e45fe1ad20fc138c877f59cdb647036c75e`  
		Last Modified: Tue, 19 Jul 2022 11:59:11 GMT  
		Size: 1.2 MB (1228014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9c4237ad9956fd1d1266bf16c5bf3e5f40ea1647c609eb353d8fd8ada94e`  
		Last Modified: Tue, 19 Jul 2022 11:59:10 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f87bfc6960c7ede1eaaa61c5fb1bbcd69f076bae3860ac134390eb2355660f24
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121499243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e7a5a42aa7a8f226d09727265221a1efb63f8143e406db52e196353e9099e23`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:49:19 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:49:20 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:49:21 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:51:30 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:52:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:53:00 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:53:01 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:53:02 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:53:03 GMT
WORKDIR /go
# Tue, 19 Jul 2022 05:24:27 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 05:24:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 05:24:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 05:24:29 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 05:24:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 05:24:33 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 05:24:33 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd11db305753e3de168e93d91f50ec724d33aa194148df6a3509dd85789f41a9`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 271.7 KB (271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64f5c91bf32af83371aee853f2f02c3bdbcbfdca89e74ffd192040c3327172b`  
		Last Modified: Mon, 18 Jul 2022 22:56:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e80723a217831e1735d1e6abdaf01331eea4ee52dc8c3d3db0a5029a256f8b`  
		Last Modified: Mon, 18 Jul 2022 22:57:29 GMT  
		Size: 110.3 MB (110291690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2774afd0c4d3ded992c58f3b5e5939d091bd26f40e507c6dc21dcbd8b7ff486f`  
		Last Modified: Mon, 18 Jul 2022 22:57:14 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4699679e405889fc7462c4d0b852cfd11aaf1195b1a1258003d50f9c934a9d56`  
		Last Modified: Tue, 19 Jul 2022 05:25:06 GMT  
		Size: 7.1 MB (7051437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c112d21408ab1ee986c071fe763b5cce6c64c2d8fbe53941ad853f8dba2980d`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 1.2 MB (1189004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2791d3bb68427e78570a5323febaa0bb744152492e53597762d31c40a888142`  
		Last Modified: Tue, 19 Jul 2022 05:25:05 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:532958fc3e446d7c88e6fd10babe06128d299a41abb4928d7e2c6018d60475ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122017996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b89bcf22d7d76306e8798211b0404616a67670b4f9c4195c99c68bd8af2463`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Wed, 27 Jul 2022 22:24:31 GMT
RUN apk add --no-cache ca-certificates
# Wed, 27 Jul 2022 22:24:33 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 27 Jul 2022 22:24:33 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:32:01 GMT
ENV GOLANG_VERSION=1.18.4
# Wed, 27 Jul 2022 22:34:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Wed, 27 Jul 2022 22:34:44 GMT
ENV GOPATH=/go
# Wed, 27 Jul 2022 22:34:45 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 27 Jul 2022 22:34:46 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Wed, 27 Jul 2022 22:34:46 GMT
WORKDIR /go
# Thu, 28 Jul 2022 09:29:36 GMT
RUN apk add --no-cache     git     ca-certificates
# Thu, 28 Jul 2022 09:29:36 GMT
ENV XCADDY_VERSION=v0.3.0
# Thu, 28 Jul 2022 09:29:36 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:37 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Thu, 28 Jul 2022 09:29:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Thu, 28 Jul 2022 09:29:39 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Thu, 28 Jul 2022 09:29:39 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a144f7bf3228ae252f9b6444da3dcdd765d01ec4540c0d5c314786fff682a8`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 274.2 KB (274204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6305f1cfd1c92a17e3eeb75b85d72ff753ecb6d0b01059e94562b0f66dbd2ac2`  
		Last Modified: Wed, 27 Jul 2022 22:47:12 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211a661bab257f5ae1d806f57e3823209459f6831bf83954bbb1b6a9acd3cece`  
		Last Modified: Wed, 27 Jul 2022 22:50:31 GMT  
		Size: 110.3 MB (110295123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fecbe2919b5d18c134e253b91234871449116d830dff37658f898de15267e4a`  
		Last Modified: Wed, 27 Jul 2022 22:50:05 GMT  
		Size: 156.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8ad829a87609b916ddffea79bd317a574dd50328252c649d475aa976251088`  
		Last Modified: Thu, 28 Jul 2022 09:30:32 GMT  
		Size: 7.5 MB (7481667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0570d3a3a8b7223844379eb879178f58d0c164da2b3f02b0f76af2f0e30ce20`  
		Last Modified: Thu, 28 Jul 2022 09:30:31 GMT  
		Size: 1.2 MB (1176364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16a41c0d17d4f1f6be934dde04aa5e2f8d35fdeec4e26d6256ac2e336f54a031`  
		Last Modified: Thu, 28 Jul 2022 09:30:30 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:466374d8c98d4acad1bf6b72d4127155fc323b310e1a6b567dcbb6358dca3399
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124315688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:944a9467efc8a3e78b0769569c94c03ff3edb63da0cb9603f21b00c136682fae`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:02:03 GMT
RUN apk add --no-cache ca-certificates
# Mon, 18 Jul 2022 22:02:04 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:02:05 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:06:54 GMT
ENV GOLANG_VERSION=1.18.4
# Mon, 18 Jul 2022 22:10:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.4.src.tar.gz'; 		sha256='4525aa6b0e3cecb57845f4060a7075aafc9ab752bb7b6b4cf8a212d43078e1e4'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Mon, 18 Jul 2022 22:11:03 GMT
ENV GOPATH=/go
# Mon, 18 Jul 2022 22:11:03 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Jul 2022 22:11:05 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Mon, 18 Jul 2022 22:11:06 GMT
WORKDIR /go
# Tue, 19 Jul 2022 07:34:34 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 19 Jul 2022 07:34:35 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 19 Jul 2022 07:34:35 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 07:34:36 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 19 Jul 2022 07:34:37 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 19 Jul 2022 07:34:38 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 19 Jul 2022 07:34:38 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61acd9c257122ba873ba33e3512e53d5601607c1da6e635d5fd4a06f44a9b06`  
		Last Modified: Mon, 18 Jul 2022 22:17:46 GMT  
		Size: 272.2 KB (272158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac068bbaa22364ba0d8b706da81e58fe5919298e79d7f8d8385e5fb3a4b6978`  
		Last Modified: Mon, 18 Jul 2022 22:17:45 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455eedd391957c5341c70cc0e71eecb045a984541e718dc3b6167b759a3d1342`  
		Last Modified: Mon, 18 Jul 2022 22:18:41 GMT  
		Size: 113.2 MB (113166096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000247fb22745203d8118c08e6aec07f7a8207b8ce7d74ab258c797dd8ca4779`  
		Last Modified: Mon, 18 Jul 2022 22:18:26 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b2de44fcaa4156eec74dc79609ec452ff6cdc6e26e4026f85b439dc1f87b95`  
		Last Modified: Tue, 19 Jul 2022 07:35:24 GMT  
		Size: 7.1 MB (7052799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8b0e3ef1cbfbd1644f7597b95e936c5777cc09dd373c13ee92889309a3ea88`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 1.2 MB (1243123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958599d297f3905bc92099c3a66b9bc677d14722b563947cf4530280ca2a0bb3`  
		Last Modified: Tue, 19 Jul 2022 07:35:23 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:61656a3c4dc45283179800b954655f7fdb6e593ea84c2dd21a57f509a897a1cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:5c72a3d9ea82e3ad57a712ed10bb7e98397cc596f55fbde3b33d93c297c83bbf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842195727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f30e7029a7c1fc78bbde2f2b8a99b7ad82ab16dd68c68ec95fd8c666f0ae893d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:32:44 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:32:45 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:32:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:32:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:34:46 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:34:47 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:35:43 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:37:29 GMT
ENV GOLANG_VERSION=1.17.12
# Tue, 12 Jul 2022 22:41:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.12.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '1bdb0e54eda6d917029f8f2d92c0eb8725aea9b9243dc53c09608eb6dbc26c7a'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:41:34 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:48:23 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:48:24 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:48:26 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:48:26 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:49:39 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:49:40 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf35cf37677487b3a6263174b47b2e2b56cd7a9e53be5c11d3c44ff42ce4500`  
		Last Modified: Tue, 12 Jul 2022 20:21:54 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeeb9d045cdffa8a8f052a2b2a83961e9c8b42408047a0e4caf49a35dec69063`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9078894caf6ef326c788d2591406f4c187fd8bb3f04777662cee4de51953442b`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:552005f37f1004b0ce2427123b219106e791fb4df589640814f54ef4cc0b8325`  
		Last Modified: Tue, 12 Jul 2022 20:21:50 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196c468260d62ca4878a4416003505afc60f2b02253764d9a9ab38e194f10d12`  
		Last Modified: Tue, 12 Jul 2022 20:21:58 GMT  
		Size: 25.5 MB (25450252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b8b80e2b89fe7312f50d8be1134a7813d8e24dfbb78b82b5ddcba129025c15`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48a66cfa3d41dc889396fcadc5aa4d650bb9b6e4bd8700436e2667186182b5a`  
		Last Modified: Tue, 12 Jul 2022 20:21:48 GMT  
		Size: 317.5 KB (317481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccce678b62c0a62e35f54ec24627360f7d3d5dc247d5503d8d71cd00a3499aa`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e1a4333adc33bec6931ca85db7791fa5391cba7ed5ebe0084e81fb99ac32b4`  
		Last Modified: Tue, 12 Jul 2022 22:55:51 GMT  
		Size: 142.7 MB (142679991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706298636ee2bf6d249966da9bc1acdab492814e07cfe4651f601a098e9ea58a`  
		Last Modified: Tue, 12 Jul 2022 22:55:11 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585bafd81397de7f7527113fc1df2d1543c0407eb4b2314321cbd536d47ad39e`  
		Last Modified: Tue, 12 Jul 2022 23:51:43 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5b76d5616012e87b7bdd22c15c0754df92c32dc389951e1bb188294e8ca5c4`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d914c9a0281c4e4fad1493874ae06a0a6bcae5b431d6720199b2ddeda2b14165`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b746eda4fc1e20c0cd865c89301d484993c4625f8bf44fabe30784beafb92d`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:054d8a3a7e3eb370c4ba441ceee544d8e097cb33e8148441f15ecf98573d9f56`  
		Last Modified: Tue, 12 Jul 2022 23:51:41 GMT  
		Size: 1.7 MB (1685722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08de844853892d80127a5a2dcb3a15016d244a6655e9857af766715118bca62f`  
		Last Modified: Tue, 12 Jul 2022 23:51:40 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:97856175998bb682fc518bdfaa61ab1eb23d732ceff5b1d5afa9d4e22dafc379
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:bcadbc0f042b714c89ec28206eb41312e52a0f6369a625825226b0369f9fa462
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2478301626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d9d14be341371d4285fd481f63f4d6ae4daf751a257d82fbbb5981754c7476d`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 19:25:41 GMT
ENV GIT_VERSION=2.23.0
# Tue, 12 Jul 2022 19:25:42 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Tue, 12 Jul 2022 19:25:43 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Tue, 12 Jul 2022 19:25:44 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Tue, 12 Jul 2022 19:26:55 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 19:26:56 GMT
ENV GOPATH=C:\go
# Tue, 12 Jul 2022 19:28:02 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 12 Jul 2022 22:18:06 GMT
ENV GOLANG_VERSION=1.18.4
# Tue, 12 Jul 2022 22:20:54 GMT
RUN $url = 'https://dl.google.com/go/go1.18.4.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'dfb93c517e050ba0cfc066802b38a8e7cda2ef666efd634859356b33f543cc49'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 12 Jul 2022 22:20:55 GMT
WORKDIR C:\go
# Tue, 12 Jul 2022 23:49:52 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:49:53 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 12 Jul 2022 23:49:54 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:49:55 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 12 Jul 2022 23:50:22 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 12 Jul 2022 23:50:23 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c455a8ac43083057f2b130da6441c55c8b2f7929352fa8fc9181dfeba0e975a`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf60d7d48bea90bda8acba13108836c16d6c677fea79c3e197cef03d538d0b1`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d543d6f6b279e33304841f24e823a975d3c147df0a85330e3213efb48732cb06`  
		Last Modified: Tue, 12 Jul 2022 20:20:44 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee37d6d08696e8206e758e401f684f3fbd1d07fb69156c6f53a42b0e94917cf`  
		Last Modified: Tue, 12 Jul 2022 20:20:43 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f5e0aa8ccbe194f893dfecf53b3ee8868463647be9d429804688f66110b6b3`  
		Last Modified: Tue, 12 Jul 2022 20:20:51 GMT  
		Size: 25.7 MB (25738019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbd09eae88a94bcd41d6ef2730aad8f7dff16e5b5402016081dace052d0b9090`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6a2ba4a24727258b5fef3a16d42f99205b6457a743e8b0ad111d83d39f153ac`  
		Last Modified: Tue, 12 Jul 2022 20:20:41 GMT  
		Size: 557.3 KB (557259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b59f1fae2726474b08ddc01fd0d6c136519d966d96f4ea3bdc2f2638de3eca06`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6f7cf06f5b2461d44530efa32eb813e761d19e9c5bd407e07aa612efe9e2e5`  
		Last Modified: Tue, 12 Jul 2022 22:50:41 GMT  
		Size: 149.8 MB (149830419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5807b8b35b58046a150bcd654242c77b07014f88070d9eea7067e47b7564ac99`  
		Last Modified: Tue, 12 Jul 2022 22:49:45 GMT  
		Size: 1.5 KB (1535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7b76ed3b1df68b41bab9b9c0542caad76c10b471d4a96517267ecb6c3c248d0`  
		Last Modified: Tue, 12 Jul 2022 23:51:58 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8cbb7b961605bc058682cee3517a82d0b325045d8fcfaeb9b943ef4b9776c`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6abd66af49add02f71f297f752f5c1faa80eeb48da62e539aeeed3a84b6691`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524f5aabcba32c91f8c6d7a0de842903606a806ca1a68a906916712e5973e657`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcdad9787f0437dd26e78be69fc9e89d4952f8a15c889c9ae4863e93f5a5caa`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.9 MB (1926037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe8d75ed6def9cead25f1c37b75c0138971a081e50113b64efdeb9bc1350e29`  
		Last Modified: Tue, 12 Jul 2022 23:51:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:7faf730343c6bd50150b13b73bac1f97886a30ae15f145e5d301c8299949bb52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:2728a7a5cc9045d475a134f9230565677fe26deb5306060a0ab766d8449f6ba4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17013282 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d954b31fe122c95e58bd7257e100408c9a17c064b065f4c723b46640b61d150c`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:21:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 19 Jul 2022 00:21:05 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 19 Jul 2022 00:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 19 Jul 2022 00:21:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 19 Jul 2022 00:21:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 19 Jul 2022 00:21:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 19 Jul 2022 00:21:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 19 Jul 2022 00:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 80
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 443
# Tue, 19 Jul 2022 00:21:09 GMT
EXPOSE 2019
# Tue, 19 Jul 2022 00:21:09 GMT
WORKDIR /srv
# Tue, 19 Jul 2022 00:21:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba0a25d662370cef41a6edf3bceddbd2bda0675eb94f8568d038b7356230396`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 291.6 KB (291612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a501877fabbb599942a33a45603240e372d191f8322b000c5aafec5a5090c4e`  
		Last Modified: Tue, 19 Jul 2022 00:21:33 GMT  
		Size: 5.8 KB (5825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c62335257e66d56f8fe9203793fb935200c4788ae2328fc7820374794f3d56`  
		Last Modified: Tue, 19 Jul 2022 00:21:36 GMT  
		Size: 13.9 MB (13916885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e4608ab095ff261532ff3818afb28725d2548a4d242c96ba13bd0e268249e6a`  
		Last Modified: Tue, 19 Jul 2022 00:21:34 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:cfed1b7a1730b6530049f91e299347b35f11e17371ebf5594b5beb6dffc1ce00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16268387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0f6502abce0924aa453af3cfe208eaed6b2cc8c5c86a0654401f4b388851557`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 20:14:12 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 20:14:14 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 20:14:15 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 20:14:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 20:14:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 20:14:21 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 20:14:22 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 20:14:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 20:14:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 20:14:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 20:14:25 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 20:14:25 GMT
EXPOSE 80
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 443
# Mon, 18 Jul 2022 20:14:26 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 20:14:27 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 20:14:27 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd55c2ffb655db030265de0f3fd76fe026e17e68d87f50465dde4f83572d2498`  
		Last Modified: Mon, 18 Jul 2022 20:15:43 GMT  
		Size: 291.8 KB (291811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c540be71e6dbd54939047b9053bb535c1f1ad83df9da6b7e9ed4d707c27e92f`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ebd5e62966b61b854fd1458e479ec41ebfca38b992919a3a4780843e1e1d94`  
		Last Modified: Mon, 18 Jul 2022 20:15:52 GMT  
		Size: 13.4 MB (13364162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b2d6bf21432c63feaa4962f64c274b569467c2f123363805fd62d3e9e85894`  
		Last Modified: Mon, 18 Jul 2022 20:15:42 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:fbe0cafdb711c8750146cf97901295bae9837679fe2ebc7e1dd9fd543bf29d57
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16056794 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1070a903222f8f7077d3ab1a896a5a95fbcdde697612a691084f49303cb55da7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:14:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:14:07 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:14:08 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:14:12 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:14:14 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:14:14 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:14:15 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:14:15 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:14:16 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:14:17 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:14:18 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:14:19 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:14:20 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:14:20 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:14:21 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9805b70d5dfc4d65e1a1e1f659dc0944494a8a6895999dc5b6cc0b2d848334a`  
		Last Modified: Mon, 18 Jul 2022 22:15:36 GMT  
		Size: 290.8 KB (290757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9745c36aa57bfd2f4a283f3fcf69f62e4ff2a9f3e14d3a6f0e5fae2d22a06a49`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 5.8 KB (5828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53157176ed62bc9624354772d3eb073499188dc4f91526e3fcabdb1108148e8e`  
		Last Modified: Mon, 18 Jul 2022 22:15:44 GMT  
		Size: 13.3 MB (13347749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aad2d41c7a719516a9ea121138080b9d1d80d21c606c87d9b5dc018ac128ae18`  
		Last Modified: Mon, 18 Jul 2022 22:15:35 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:7542ee62db8e10442071d4e9745bcd98f39619bcf9f516c1c9b4ecfc5cc0f3d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15721249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db56606eb0d00c279248ae38995824f79f994477565532beb03699a02e7f94af`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 22:18:30 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 22:18:32 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 22:18:33 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 22:18:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 22:18:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 22:18:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 22:18:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 22:18:39 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 22:18:40 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 22:18:41 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 22:18:42 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 22:18:43 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 22:18:44 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 22:18:45 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 22:18:46 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 22:18:47 GMT
EXPOSE 80
# Mon, 18 Jul 2022 22:18:48 GMT
EXPOSE 443
# Mon, 18 Jul 2022 22:18:49 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 22:18:50 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 22:18:51 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a6867c1bed7442ba6f8c33877f0a64552b8eb6e640825b2b39521a3ee4d3b7`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 291.5 KB (291464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9d0dc3dac6c9ea9c214169993cbf654f21972b33784651a2e35c75b2c3332`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 5.8 KB (5751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0818fab46ac8ba80668e14951d7ac785048f4df50fda97f61507062a61e3b1ad`  
		Last Modified: Mon, 18 Jul 2022 22:19:28 GMT  
		Size: 12.7 MB (12729160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef202eac441dd743baac9767af96c921d6a74c7b67ddb0da6989963669cc967`  
		Last Modified: Mon, 18 Jul 2022 22:19:26 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:d4ed904cc09a91c433a9ef0c27b7daad6550e02f6a4ec80f2bcc2b5bfb011d64
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15399410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf5a90d8199b6618c768f8040a3f1cdb2a154789fa6612c7f6daf9362344d62`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Thu, 28 Jul 2022 09:29:14 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 28 Jul 2022 09:29:16 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 28 Jul 2022 09:29:17 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 28 Jul 2022 09:29:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 28 Jul 2022 09:29:21 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 28 Jul 2022 09:29:22 GMT
ENV XDG_DATA_HOME=/data
# Thu, 28 Jul 2022 09:29:22 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 28 Jul 2022 09:29:23 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 28 Jul 2022 09:29:24 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 80
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 443
# Thu, 28 Jul 2022 09:29:25 GMT
EXPOSE 2019
# Thu, 28 Jul 2022 09:29:26 GMT
WORKDIR /srv
# Thu, 28 Jul 2022 09:29:26 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143cf45bb3764aa69910cc3bf88d9796600ad505fe7af4d3c67695d3531cea7b`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 294.0 KB (293972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97069a68d5f45ed80b3cf6952f9b94df5d5b2010f5ba70d24213b45cc2f7477`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 5.8 KB (5833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee64bce4f5dd3491e75b5b2531cef2c68bc6cf0923aed600cf5b2c6549fa56ba`  
		Last Modified: Thu, 28 Jul 2022 09:30:15 GMT  
		Size: 12.3 MB (12309528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec473101201222cbe558f78a93799ab07b4b225382711f56d995cfb848bf5c6`  
		Last Modified: Thu, 28 Jul 2022 09:30:12 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:28adfc1e1d82c412767e4b170580d554b8dbb36c1cb5b355005e2dc8c2eeb0b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16339412 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a387c6224fd249160f6c2f8ffd24f60c57c927a1a599ce91609c9c27288434c7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:02:21 GMT
RUN apk add --no-cache ca-certificates mailcap
# Mon, 18 Jul 2022 21:02:24 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Mon, 18 Jul 2022 21:02:25 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 18 Jul 2022 21:02:32 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Mon, 18 Jul 2022 21:02:36 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Mon, 18 Jul 2022 21:02:37 GMT
ENV XDG_CONFIG_HOME=/config
# Mon, 18 Jul 2022 21:02:38 GMT
ENV XDG_DATA_HOME=/data
# Mon, 18 Jul 2022 21:02:38 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Mon, 18 Jul 2022 21:02:39 GMT
LABEL org.opencontainers.image.title=Caddy
# Mon, 18 Jul 2022 21:02:40 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Mon, 18 Jul 2022 21:02:41 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Mon, 18 Jul 2022 21:02:42 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Mon, 18 Jul 2022 21:02:43 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Mon, 18 Jul 2022 21:02:44 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 80
# Mon, 18 Jul 2022 21:02:45 GMT
EXPOSE 443
# Mon, 18 Jul 2022 21:02:46 GMT
EXPOSE 2019
# Mon, 18 Jul 2022 21:02:46 GMT
WORKDIR /srv
# Mon, 18 Jul 2022 21:02:47 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01286e5b65105b357bf83e8daa3cbc0a1a069a4d14af918fcd5475246f6af1b`  
		Last Modified: Mon, 18 Jul 2022 21:03:38 GMT  
		Size: 291.9 KB (291948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ce119bc29da400dd00bd331789e14fab9587661da4bb3e57835053afeb50b7`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 5.8 KB (5826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8470e2e663127d3838fb96d9115f33c868c378cea548725085b75d9f39599548`  
		Last Modified: Mon, 18 Jul 2022 21:03:40 GMT  
		Size: 13.5 MB (13460687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e115a0286c47b77821e5d98da581e1d3e1f85b3dd134111f6c27790d0c45fbae`  
		Last Modified: Mon, 18 Jul 2022 21:03:37 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:a6506a1cb644e10461e5a43a0514aef50d49a62d898aa73e9c3604ecfc697cb2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3165; amd64
	-	windows version 10.0.20348.825; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:744553df106b3067f1d20b1b0c6431c3b6fa66c99b0fabe0cd9518beecbad6ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:16c79973fbcf50574de31aa302119726c02b34fdb88d43f1f074e88464872845
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2686983922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53af60fd100e235d28b984cabce660df5f8e18c565c0f3b7d4b794af79fae42`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:41:08 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:41:09 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:43:34 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:43:36 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:43:38 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:43:40 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:43:43 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:43:46 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:43:48 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:43:51 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:43:53 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:43:55 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:43:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:43:59 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:44:01 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:44:03 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:45:55 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:45:56 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0fcaa03f4055407c03fde1a3d7451b52c56d40c085923a2417f37ec4bf4d55`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 364.3 KB (364306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c4a38ea4791b667f2ac030f375bd051a1e740a2bae5e596412fc5b2545fb0e`  
		Last Modified: Tue, 12 Jul 2022 23:51:00 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2531a821edb829f6e0ecb4b742264a3f2c21cb05fe7d2643732bbd87777b589e`  
		Last Modified: Tue, 12 Jul 2022 23:51:03 GMT  
		Size: 14.2 MB (14245014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41c345f103368119f5bbc78ae48e434cfd6210009fc64c1ab7f6cb79ffc5074`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c48344f8c370e0ba5f36cdbd92676e0b3785f98370ad579a398b8466baf86e6`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96b22f34f05e7b9dca8dc17d51b5af14f27c2a4c5f9b7163fbe68194f05f95`  
		Last Modified: Tue, 12 Jul 2022 23:50:58 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9be0565ea1f98b668ca40d5c317d72fe7be6253e9822cb061364356fa81c02d`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c77c9eb4e4e8603825bf36b921061eeacf19c7699e58d9e4c981cbb5616c96`  
		Last Modified: Tue, 12 Jul 2022 23:50:57 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0625f6896d40089006f37ec00ab3e22ef89ec5a215b58514da23f4a3b054bd3c`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1814d4ff3888ea3223be9648585feb7a6edd3003bd6b0ef67d95589d6268eb1`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb385b6e63236c0bbcaf5837075fef88af445a0131e80818373f0be4492d3b3`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1786fe541fc44e1c45c5acb9b1c1392978694eb03515af3c1c98ec84d4a53eb`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd961e85021eadf6a22e7cd7c2273685be0df9fccc6ca72dffa40106ac72235`  
		Last Modified: Tue, 12 Jul 2022 23:50:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4757593a7356e21b5a441a5fc9e66f3a3d7f79ecb4b064f7bd7866152e59af53`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfd2162b126838c72e7fda55b4910c9bd3b7844e673098fd338c34a621eb5`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7a069076f80a1f9c9bdc79e54a2346fbfe61f08cc6fa3086bf913bfb5c9811`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1208e7bc2dab41d5a22bc4458bcdb4d4772ef77958ad5055931fb1ec857963`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 308.2 KB (308223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf8d7e52b3992a4c097987ce0219a718c817f66ffd2507230735356a75889b4`  
		Last Modified: Tue, 12 Jul 2022 23:50:53 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:4b56a1d12cc2f346deceebca9dca6640d81a1ca369c68151f5dd2d9c3ffccbbe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.825; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.825; amd64

```console
$ docker pull caddy@sha256:70b310a2587b0b5cd9108c4d22292e7a61783e0c924e70342275761d345a928e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2315742699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0fbcbee02efa576a28f6127461c2e72eec33d22cb952ea66829c14cdbf70b24`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Mon, 04 Jul 2022 17:46:55 GMT
RUN Install update 10.0.20348.825
# Tue, 12 Jul 2022 19:25:40 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 12 Jul 2022 23:46:54 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Tue, 12 Jul 2022 23:46:55 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 12 Jul 2022 23:47:26 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Tue, 12 Jul 2022 23:47:27 GMT
ENV XDG_CONFIG_HOME=c:/config
# Tue, 12 Jul 2022 23:47:29 GMT
ENV XDG_DATA_HOME=c:/data
# Tue, 12 Jul 2022 23:47:30 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 12 Jul 2022 23:47:31 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 12 Jul 2022 23:47:32 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 12 Jul 2022 23:47:33 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 12 Jul 2022 23:47:34 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 12 Jul 2022 23:47:35 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 12 Jul 2022 23:47:36 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 12 Jul 2022 23:47:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 12 Jul 2022 23:47:38 GMT
EXPOSE 80
# Tue, 12 Jul 2022 23:47:39 GMT
EXPOSE 443
# Tue, 12 Jul 2022 23:47:40 GMT
EXPOSE 2019
# Tue, 12 Jul 2022 23:48:02 GMT
RUN caddy version
# Tue, 12 Jul 2022 23:48:03 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e1a27cb9d4615dec325f2cbabac4ca1f65413bdbb8b440cc961df032993a9b81`  
		Size: 863.4 MB (863367943 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6452cb934201756f0ed9fb5e0cbea54a22a66412cb696ff30a1923d456e28bcf`  
		Last Modified: Tue, 12 Jul 2022 20:20:48 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6accfb6a5659ca8200a6936ffc29bd07a86f82f121b29db78aa49a2602cb53cf`  
		Last Modified: Tue, 12 Jul 2022 23:51:24 GMT  
		Size: 662.7 KB (662655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76563f9ad165ff1b1e4169684deeaa7e3ebeb2c4e216a5bf897e4808e78b97ad`  
		Last Modified: Tue, 12 Jul 2022 23:51:23 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d87f5055f9b1ffb3e26749ff66ba716bc365fa62c5107185a7da1bbead0e8f`  
		Last Modified: Tue, 12 Jul 2022 23:51:27 GMT  
		Size: 14.5 MB (14483857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e860443f38114e05bd48860d9cdbee14662f341736b036bcf5ea64a909bd841d`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2938a7653cb825d868eeb02a0cf03b6ae61097f91bbbdd9655c726079e5f17`  
		Last Modified: Tue, 12 Jul 2022 23:51:22 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0488511aac98e33847a54aed263475b6fb9da107d4c72879e4b072b55f5eeb`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db2317adf16d33e16b56a17e7bb64e74aec0b7fee5efb829f17b25f520996d4`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acaf703fec200ee27f7395e3c4859dbcea9f532e726441e62ca812c0edd2302`  
		Last Modified: Tue, 12 Jul 2022 23:51:21 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f374937095259775156a5a5972510f5f800a799864c30e6bf949e9950f6ef1f5`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a31f89fc0e9591c89dc5f1f4684281e31fd17c5776b20bd5750113cc57c5450`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d812209c52ba6103b7181921c021108025f67b21142e14e14343526949b63`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2ad97b6c1c9140023c578499123559016f89056c57dcb14b01e27831eaff4f`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be35a9de6e1e90ebb55512a4843550ca2bf1073b26f4ae8be25f63ae29f30da`  
		Last Modified: Tue, 12 Jul 2022 23:51:19 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf9e3b5eeeb22314c8a06148cdff4400e3a898e6666cb26f3503b9b3dff1987`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a979d5f3d61b7a30b697a5e5c5d7084d919ea418e7667ed60d7e5498e49836f`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f53ba99eb618fa7b22aaeb283d73e0b2adc339ee2b74e4d74015c7172996b0d`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19a42d65298123fbf06b0b4d2419e783d50075a9d4c668ca739ca1d468ea30d`  
		Last Modified: Tue, 12 Jul 2022 23:51:17 GMT  
		Size: 341.9 KB (341931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0726092d61b296edc9e242276b83fb08dcb5b18b9d5e96fb00d99cb0571a66c`  
		Last Modified: Tue, 12 Jul 2022 23:51:16 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
