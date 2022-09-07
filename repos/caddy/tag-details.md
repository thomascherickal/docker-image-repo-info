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
-	[`caddy:2.6.0-beta.3`](#caddy260-beta3)
-	[`caddy:2.6.0-beta.3-alpine`](#caddy260-beta3-alpine)
-	[`caddy:2.6.0-beta.3-builder`](#caddy260-beta3-builder)
-	[`caddy:2.6.0-beta.3-builder-alpine`](#caddy260-beta3-builder-alpine)
-	[`caddy:2.6.0-beta.3-builder-windowsservercore-1809`](#caddy260-beta3-builder-windowsservercore-1809)
-	[`caddy:2.6.0-beta.3-builder-windowsservercore-ltsc2022`](#caddy260-beta3-builder-windowsservercore-ltsc2022)
-	[`caddy:2.6.0-beta.3-windowsservercore`](#caddy260-beta3-windowsservercore)
-	[`caddy:2.6.0-beta.3-windowsservercore-1809`](#caddy260-beta3-windowsservercore-1809)
-	[`caddy:2.6.0-beta.3-windowsservercore-ltsc2022`](#caddy260-beta3-windowsservercore-ltsc2022)
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
$ docker pull caddy@sha256:740c1c9e461ea1f8a54d7512b35cd31927c814c86455f71e7e8e0c2b6ee423a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2` - linux; amd64

```console
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-alpine`

```console
$ docker pull caddy@sha256:39efb1f71eaf6390e2241c00ddd8dc6242cdcb4149abf06050c0a9ebcc773838
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
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder`

```console
$ docker pull caddy@sha256:3659712be2191d3e6d5f6d174b3a6a7374029cc29b88c603d515ea955f54e479
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
	-	windows version 10.0.20348.887; amd64

### `caddy:2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-alpine`

```console
$ docker pull caddy@sha256:9ef62ec1134cd523777caad619988b02e90554c28c267edb66c1afead33ed41b
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
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:eb601da6d7c5be6870705ba00b8894f554a1ce85e1b4951b4a0ed135ec392a26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2-builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:fe0d29bba97b1d3dc69101d71a946a9c287ae54e09bf74ceda0862cbcc9c8c01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore`

```console
$ docker pull caddy@sha256:d98344a194f90621248b3c94ba8b3c2fe4cbc4ee05cfc22334d2a747cb2350bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:0390ac5f55f7a6eae2a40f9256802bc1c6bbe33a01f41ed73b0d932c91f76f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:ce2b42e067d32df033d35738362e9279cbb832f91d400e14a9dd2c5d2e50c1eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2`

```console
$ docker pull caddy@sha256:740c1c9e461ea1f8a54d7512b35cd31927c814c86455f71e7e8e0c2b6ee423a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2` - linux; amd64

```console
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-alpine`

```console
$ docker pull caddy@sha256:39efb1f71eaf6390e2241c00ddd8dc6242cdcb4149abf06050c0a9ebcc773838
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
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder`

```console
$ docker pull caddy@sha256:3659712be2191d3e6d5f6d174b3a6a7374029cc29b88c603d515ea955f54e479
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
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-builder` - linux; amd64

```console
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-alpine`

```console
$ docker pull caddy@sha256:9ef62ec1134cd523777caad619988b02e90554c28c267edb66c1afead33ed41b
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
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:eb601da6d7c5be6870705ba00b8894f554a1ce85e1b4951b4a0ed135ec392a26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:2.5.2-builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:fe0d29bba97b1d3dc69101d71a946a9c287ae54e09bf74ceda0862cbcc9c8c01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore`

```console
$ docker pull caddy@sha256:d98344a194f90621248b3c94ba8b3c2fe4cbc4ee05cfc22334d2a747cb2350bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:2.5.2-windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-1809`

```console
$ docker pull caddy@sha256:0390ac5f55f7a6eae2a40f9256802bc1c6bbe33a01f41ed73b0d932c91f76f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:2.5.2-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.5.2-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:ce2b42e067d32df033d35738362e9279cbb832f91d400e14a9dd2c5d2e50c1eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:2.5.2-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:2.6.0-beta.3`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-alpine`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-builder`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-builder-alpine`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-builder-windowsservercore-1809`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-builder-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-windowsservercore`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-windowsservercore-1809`

**does not exist** (yet?)

## `caddy:2.6.0-beta.3-windowsservercore-ltsc2022`

**does not exist** (yet?)

## `caddy:alpine`

```console
$ docker pull caddy@sha256:39efb1f71eaf6390e2241c00ddd8dc6242cdcb4149abf06050c0a9ebcc773838
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
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:alpine` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder`

```console
$ docker pull caddy@sha256:3659712be2191d3e6d5f6d174b3a6a7374029cc29b88c603d515ea955f54e479
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
	-	windows version 10.0.20348.887; amd64

### `caddy:builder` - linux; amd64

```console
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-alpine`

```console
$ docker pull caddy@sha256:9ef62ec1134cd523777caad619988b02e90554c28c267edb66c1afead33ed41b
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
$ docker pull caddy@sha256:5be78595011dad61eedef58283a3e724cb7bb97adb161a4c72b2459b6be7d1e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.7 MB (126656074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a613f2306c18908a90e4e6f721dd6da4fc2ea19bc34e1a74ab10d1fd88853222`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:11:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:11:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:11:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:56 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:33 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:33 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:33 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:34 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:01 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:01 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:01 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:02 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:02 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:03 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5299e6f7860564fd4df7e9a224f3d05dc26d0e855fb26ac7e9d9e156cf1422b2`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 284.7 KB (284725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cab0e43db0af1d30e55de347bd78df438344691f8fb379f631a07e2c8a80f0a`  
		Last Modified: Tue, 09 Aug 2022 19:19:30 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548b71e657dcad90931c40bcff39aa8b21c33ac888ac08ee16e6bc3577a16264`  
		Last Modified: Tue, 06 Sep 2022 19:32:56 GMT  
		Size: 115.3 MB (115333545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0792f1a6db3731fdacdd2e3bd0976d8ff18a913795f8afd8f3c5ecd279b874d`  
		Last Modified: Tue, 06 Sep 2022 19:32:40 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac41a3b93e7a2c16abdd01df0f5fdf5af587ff67302d0e0d6b7dbffd32f3040`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 6.9 MB (6941626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23c19c2e109af7dd1b25e28bda078cdc0ed928dfdec9fe14cb73a4f7db22d17d`  
		Last Modified: Tue, 06 Sep 2022 19:53:21 GMT  
		Size: 1.3 MB (1289409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98371edebfa24727ea5e91648b3b7bdd59bfea04e9b319c3939c7998c97b2a12`  
		Last Modified: Tue, 06 Sep 2022 19:53:20 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v6

```console
$ docker pull caddy@sha256:fbc077837c8128621d7fcfdab486f7fb07690b6045e3ae06264fe135311e6592
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122651927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b042e8b10c1c1d07fbc994569f1f0a74623cada8155614fe9dc38d1f5c522b05`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:55:06 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:55:07 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:55:07 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:04:41 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:10:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:10:47 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:10:47 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:10:47 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:10:47 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:36:28 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:36:28 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:36:28 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:36:29 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:36:29 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:36:29 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d9c949f49fc8f526d6efc5da6670075476f51650be8b4471ba9b4b6e23b2ba`  
		Last Modified: Tue, 09 Aug 2022 19:19:26 GMT  
		Size: 284.7 KB (284675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63f78ae51a196097165b296ccc0c98c86e0a59180d1b4a8020fc88ec6b19f9e`  
		Last Modified: Tue, 09 Aug 2022 19:19:25 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318579c6aa9fa274f5a95fc05d75ab278e5b04beed1088990d3a7772305dbff4`  
		Last Modified: Tue, 06 Sep 2022 19:20:09 GMT  
		Size: 111.7 MB (111715273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89ab55d59c284f07f4d4f0bd0bef5e72491a6949efa65cc2842988a2ee21096`  
		Last Modified: Tue, 06 Sep 2022 19:19:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e611c962e5b711527d3e765e693e0872d5e2b5f84a900d6c2fd6cf83bb5891f`  
		Last Modified: Tue, 06 Sep 2022 19:37:07 GMT  
		Size: 6.8 MB (6808141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a7c8692e6f8a9baa5abbcd18fb66d9b87a612f259302e3bc0134b919d48aa0`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 1.2 MB (1229159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb234f1f98a7d2a736ee36e42f10ae7a8dea8fe86f7c4d2d7d8faf689b5d5e7`  
		Last Modified: Tue, 06 Sep 2022 19:37:06 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm variant v7

```console
$ docker pull caddy@sha256:9d20896516d9a487c1d96fbed578797c03b12309d0305f513595f9cedc293b28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.5 MB (121489424 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a347ea9850a53db65ac83be8c33223046c5ebe50a8af94e6fbee18c7533fbcf4`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:39:16 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:39:17 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:39:17 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:14:18 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:19:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:19:27 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:19:27 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:19:27 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:19:27 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:48:18 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:48:18 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:48:18 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:48:19 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:48:19 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:48:20 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f798709c06b1d0d785a75093457bb4ec2c7f376b428c2cf241ac3bd6439cc66`  
		Last Modified: Tue, 09 Aug 2022 19:02:41 GMT  
		Size: 283.8 KB (283817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c90e18713445588346a44b856414285a0246c86da6eb9ec2597761b27a9f27a4`  
		Last Modified: Tue, 09 Aug 2022 19:02:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec55af50bb3ab213dca9c22c088def5cc4f2aed8d1b1d15e22deebb0615de800`  
		Last Modified: Tue, 06 Sep 2022 19:29:31 GMT  
		Size: 111.5 MB (111492014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8655b299f19a59bcb51c5976e4c36cf1f21cc342082676cd9bc36532be7c174b`  
		Last Modified: Tue, 06 Sep 2022 19:29:11 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9121da58bd4a254837163cbe4535a4455bc3dfa297b208f286d6c92ab3b0a`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 6.1 MB (6067797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8af4e698d72a6e3510d9125a288694a45557d471bf3e3e1c14fccb1a9656969f`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 1.2 MB (1228018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36258acdb4751f8fed44166894f522d662f444c5e90e10ba3d55240423beb9fc`  
		Last Modified: Tue, 06 Sep 2022 19:48:57 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:5fbb02ec853a9985d6cc10e87b1c5bbd9cb7524631bf48baf059a85ae3085ea1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.6 MB (121600857 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:705ace040f7dda2f21d43ac983eb1eb440a3f1bbf5dcfdc55502d6c7e8f0c778`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:07:56 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 19:07:57 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 19:07:58 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:02:20 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 20:03:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 20:03:53 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 20:03:53 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 20:03:54 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 20:03:55 GMT
WORKDIR /go
# Tue, 06 Sep 2022 21:07:31 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 21:07:32 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 21:07:33 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 21:07:34 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 21:07:36 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 21:07:37 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 21:07:37 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817a8a8f634c3a78b1a3b55a03335868971f2378932d3454ece4e3bfc5931675`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 284.5 KB (284523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4392115cee3dde58f6f650f24b78fb0a4dd12537cca1b3eec0be6ffb470055aa`  
		Last Modified: Tue, 09 Aug 2022 19:16:28 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9cc886a859608c27b30d16ebc98fed7f82df460d4ab15abfb8d4f61eeb5386`  
		Last Modified: Tue, 06 Sep 2022 20:10:22 GMT  
		Size: 110.4 MB (110366710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bedf62e8a28797350d6cf6110ed0f8a7c85a64a825bbdf33ebbde238b363a67`  
		Last Modified: Tue, 06 Sep 2022 20:10:07 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee1ff7d11bb6bee5220a2d649d7080b2ee50a80b97459e5fca4be3e29bcaa5b`  
		Last Modified: Tue, 06 Sep 2022 21:08:11 GMT  
		Size: 7.1 MB (7052270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2870174d367419348e5ad4657c902c937f16eb9737b6a886258825f9d479d347`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 1.2 MB (1189007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15c4f0d97c3723cc39f001fdfc0c62d9e4edad8d432fa13b51376fd03665b7b4`  
		Last Modified: Tue, 06 Sep 2022 21:08:10 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; ppc64le

```console
$ docker pull caddy@sha256:38b96afb05a6661327754fce884241e117304b26fd2794cecb3f8a05a9e8b5a6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122145249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbbb3eb4df745ce8dc169f4f9937b663ff24735aa2c2c79e1152799d00e5ff9f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:01 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:15:02 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:02 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:24:11 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:26:54 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:26:55 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:26:56 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:26:56 GMT
WORKDIR /go
# Tue, 06 Sep 2022 19:53:40 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 19:53:40 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 19:53:41 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 19:53:41 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 19:53:43 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 19:53:43 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 19:53:43 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0369baf68c186e68d7c3cee256f5bc3a9351c6763ed88a03033834a5b942b700`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 286.7 KB (286735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63509bba13834179c96797234162e3d1ecb1e36f10462a0843db700ff48f1657`  
		Last Modified: Tue, 09 Aug 2022 18:28:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35cb6c0cf0353cdf77d4c9c56145c14be603eb81cc01a6a8539a24a61eba24ac`  
		Last Modified: Tue, 06 Sep 2022 19:34:36 GMT  
		Size: 110.4 MB (110395852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ed50f057913f3ef8d15429da9385fdf32c67ea04baa53b921edcc15eb9453`  
		Last Modified: Tue, 06 Sep 2022 19:34:10 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fc5144a585f8aa1a69e4697a0ac8dc7b7004bb31e2898200a7185245992e61`  
		Last Modified: Tue, 06 Sep 2022 19:54:20 GMT  
		Size: 7.5 MB (7482258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331ea735182dd2d45ae5c5cb907bacba9cccd989fdf2db64927f430d7aec7339`  
		Last Modified: Tue, 06 Sep 2022 19:54:19 GMT  
		Size: 1.2 MB (1176370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e3c343a154b2750cd3240f0385b7a981f9de471d00f2a8bfd23f78a35979e1`  
		Last Modified: Tue, 06 Sep 2022 19:54:18 GMT  
		Size: 405.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:builder-alpine` - linux; s390x

```console
$ docker pull caddy@sha256:59e72031fb975a03059d9ca1decc3d397aef3e9e67b5c393bdd314d73574d039
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124389978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c6f17616ccf44db992d96732b95fd6593406e283536b796efe3dab0c5cd1df4d`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:45:21 GMT
RUN apk add --no-cache ca-certificates
# Tue, 09 Aug 2022 18:45:22 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:45:22 GMT
ENV PATH=/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:53:27 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:55:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps gnupg; 	arch="$(apk --print-arch)"; 	url=; 	case "$arch" in 		'x86_64') 			export GOAMD64='v1' GOARCH='amd64' GOOS='linux'; 			;; 		'armhf') 			export GOARCH='arm' GOARM='6' GOOS='linux'; 			;; 		'armv7') 			export GOARCH='arm' GOARM='7' GOOS='linux'; 			;; 		'aarch64') 			export GOARCH='arm64' GOOS='linux'; 			;; 		'x86') 			export GO386='softfloat' GOARCH='386' GOOS='linux'; 			;; 		'ppc64le') 			export GOARCH='ppc64le' GOOS='linux'; 			;; 		's390x') 			export GOARCH='s390x' GOOS='linux'; 			;; 		*) echo >&2 "error: unsupported architecture '$arch' (likely packaging update needed)"; exit 1 ;; 	esac; 	build=; 	if [ -z "$url" ]; then 		build=1; 		url='https://dl.google.com/go/go1.18.6.src.tar.gz'; 		sha256='a7f1d50424355dabce66d1112b1cae439b6ee5e4f15edba6f104c0a4b173e895'; 	fi; 		wget -O go.tgz.asc "$url.asc"; 	wget -O go.tgz "$url"; 	echo "$sha256 *go.tgz" | sha256sum -c -; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 'EB4C 1BFD 4F04 2F6D DDCC  EC91 7721 F63B D38B 4796'; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys '2F52 8D36 D67B 69ED F998  D857 78BD 6547 3CB3 BD13'; 	gpg --batch --verify go.tgz.asc go.tgz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" go.tgz.asc; 		tar -C /usr/local -xzf go.tgz; 	rm go.tgz; 		if [ -n "$build" ]; then 		apk add --no-cache --virtual .build-deps 			bash 			gcc 			go 			musl-dev 		; 				export GOCACHE='/tmp/gocache'; 				( 			cd /usr/local/go/src; 			export GOROOT_BOOTSTRAP="$(go env GOROOT)" GOHOSTOS="$GOOS" GOHOSTARCH="$GOARCH"; 			./make.bash; 		); 				apk del --no-network .build-deps; 				rm -rf 			/usr/local/go/pkg/*/cmd 			/usr/local/go/pkg/bootstrap 			/usr/local/go/pkg/obj 			/usr/local/go/pkg/tool/*/api 			/usr/local/go/pkg/tool/*/go_bootstrap 			/usr/local/go/src/cmd/dist/dist 			"$GOCACHE" 		; 	fi; 		apk del --no-network .fetch-deps; 		go version
# Tue, 06 Sep 2022 19:55:12 GMT
ENV GOPATH=/go
# Tue, 06 Sep 2022 19:55:12 GMT
ENV PATH=/go/bin:/usr/local/go/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 06 Sep 2022 19:55:12 GMT
RUN mkdir -p "$GOPATH/src" "$GOPATH/bin" && chmod -R 777 "$GOPATH"
# Tue, 06 Sep 2022 19:55:13 GMT
WORKDIR /go
# Tue, 06 Sep 2022 20:21:05 GMT
RUN apk add --no-cache     git     ca-certificates
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:21:05 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:21:05 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:21:06 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='889b63098037e4641cce5b355bd82535a4b6bbbc4aa16b8214108d0d847d288b52cd19017a477eedc9c066c2ec623310dd7909251888bc9432a7d7553ba9037e' ;; 		armhf)   binArch='armv6'; checksum='decfc298b900b62ee16e0dc92a05d3b61926b961de5ee10138ce9fc6cde85dba732928d4481e02e4290750c85a92c4c24c1850045eb16c0d6a75781ff1506964' ;; 		armv7)   binArch='armv7'; checksum='99819ca7b2d37ab93e0b6af8f41dbc16dec5844c47b64993c1c1c2df0567e4abbff55ca6e9642231bd68a1789d0ebbef36822362f0c29d6dcdb01d55b3669cba' ;; 		aarch64) binArch='arm64'; checksum='24203b66ed47ba5aaa358a9e84c6a13f48737d8dc2902fdc7e2218409ac1bde9f043f0bbdf7b66697c9f9263cf1272a73784e51a26eca94ff37bcda4c21ece87' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='b96d1e6bfced6288678d45b120988e0c9e386671526688d229ace91b8f40ae03ae98a31aca9bdbbdbb9b865037e606801e434594d49cb1654398f53b4f904fd4' ;; 		s390x)   binArch='s390x'; checksum='6af5190825ac0ff01a60c7bfe5dbfea999841b9b1cf8dfca337c30eabc4aa7c03ad4da948f3472954a94f53552c1ab0a7bbd76894af6eb218ae118de68481f78' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/xcaddy.tar.gz "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/xcaddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/xcaddy.tar.gz -C /usr/bin xcaddy; 	rm -f /tmp/xcaddy.tar.gz; 	chmod +x /usr/bin/xcaddy;
# Tue, 06 Sep 2022 20:21:06 GMT
COPY file:3284b89c053fa1b60b278653bdca42a092891284e07e11d2fe66ee30b14e3081 in /usr/bin/caddy-builder 
# Tue, 06 Sep 2022 20:21:06 GMT
WORKDIR /usr/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3e6b82e3d7aa395eb79202f28debe691c40472030a94ade061f395a44b1cfa`  
		Last Modified: Tue, 09 Aug 2022 18:55:04 GMT  
		Size: 284.9 KB (284946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b3e76524e71d305c75cb023708a1803b53b20a32bef9a06fd0554590d17ab3`  
		Last Modified: Tue, 09 Aug 2022 18:55:05 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c2c0966068a4226441db01c49f3e23353d696b5f7247c665b719b364173f77`  
		Last Modified: Tue, 06 Sep 2022 20:00:07 GMT  
		Size: 113.2 MB (113217637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c44dc513c74979986f9dd3815c88c8fbb11fd3389b1e571664c4659da96ee93`  
		Last Modified: Tue, 06 Sep 2022 19:59:53 GMT  
		Size: 157.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7334145d2167491bcab4aa7825e71adc730f2e19a2fd33a3d821ab322022d0f`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 7.1 MB (7052958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a42d8dbfb01353c714283dfd3bddaa96a056c076904f647cb5fb8c2ae4c9af`  
		Last Modified: Tue, 06 Sep 2022 20:21:43 GMT  
		Size: 1.2 MB (1243126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c8e5f942f35f83c5097698e95a4617e02a243f57f03acb8e81e7acb3bf31aa`  
		Last Modified: Tue, 06 Sep 2022 20:21:42 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-1809`

```console
$ docker pull caddy@sha256:eb601da6d7c5be6870705ba00b8894f554a1ce85e1b4951b4a0ed135ec392a26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `caddy:builder-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull caddy@sha256:221bec1bb1634d52575e34a1a84cea97f3af3c87795273d77783b88a7c3f17b0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2842283253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b7cdec919451c396c03da53e34a6c3c5a57328cdb302572c6c0231685034cf9`
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
# Mon, 01 Aug 2022 16:35:39 GMT
ENV GOLANG_VERSION=1.17.13
# Mon, 01 Aug 2022 16:39:32 GMT
RUN $url = 'https://dl.google.com/go/go1.17.13.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '6cea8e199c8034995f3a691ef4564e0cc6645ee1649d7ef268a836387f1a5dfa'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Mon, 01 Aug 2022 16:39:34 GMT
WORKDIR C:\go
# Mon, 01 Aug 2022 17:12:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Mon, 01 Aug 2022 17:12:02 GMT
ENV XCADDY_VERSION=v0.3.0
# Mon, 01 Aug 2022 17:12:03 GMT
ENV CADDY_VERSION=v2.5.2
# Mon, 01 Aug 2022 17:12:04 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Mon, 01 Aug 2022 17:13:11 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Mon, 01 Aug 2022 17:13:12 GMT
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
	-	`sha256:4c6786a44e0c6c0a90653689194ad071badd6cc53ede736a8d756f72427b6efb`  
		Last Modified: Mon, 01 Aug 2022 16:52:20 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea57d5983ffc59d3feac079a134b1e3225a758d74208aa012fe0a8d53198a820`  
		Last Modified: Mon, 01 Aug 2022 16:52:52 GMT  
		Size: 142.7 MB (142747249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9433e9e494c73efd50f582d4728438df6e0baa49cec36df6bd408edf97dda9`  
		Last Modified: Mon, 01 Aug 2022 16:52:21 GMT  
		Size: 1.6 KB (1585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1525a52991673f9213129a92dcf3bd5102e6e31395862dd7ac1f9441191184c`  
		Last Modified: Mon, 01 Aug 2022 17:14:44 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b53f286b6f30ee8d87a0b4710908b6bed0049d554f649e8677222ad62d5467`  
		Last Modified: Mon, 01 Aug 2022 17:14:41 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf43fd2bba84cd29eaf59f4e072b01904af867e4b0426354634170a09bfb435e`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d45f9e8361e67da6ca9560b07c35dd6148086b41eb8ed4ce7aa378c4758d7cb`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c2dac65121eb597e696c9fba1031708253a585edb8a600ae72a0c716a9d950`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.7 MB (1705998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:437ec56cf9c73cd8802bf0cb2f8882ee7f09a7a32093081f92b364d0ff502753`  
		Last Modified: Mon, 01 Aug 2022 17:14:42 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:builder-windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:fe0d29bba97b1d3dc69101d71a946a9c287ae54e09bf74ceda0862cbcc9c8c01
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:builder-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:74e5c262569cc62e28d6a0c26d55b346fe44a6e237885f79cd046dc67e8feee9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2495017603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0cdfe05622c54c44a1ea1396c550b4a927c74c0d24e8e2ac3bb5438ab3a7dfb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:49:45 GMT
ENV GIT_VERSION=2.23.0
# Wed, 10 Aug 2022 12:49:46 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 10 Aug 2022 12:49:47 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 10 Aug 2022 12:49:48 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 10 Aug 2022 12:50:18 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 12:50:19 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 12:50:39 GMT
RUN $newPath = ('{0}\bin;C:\Program Files\Go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 06 Sep 2022 19:32:19 GMT
ENV GOLANG_VERSION=1.18.6
# Tue, 06 Sep 2022 19:35:26 GMT
RUN $url = 'https://dl.google.com/go/go1.18.6.windows-amd64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = '480b7212ab1d152d5e3fc382ac34d3dd26bf637ae4537c35b4b554ede8a36b47'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Moving ...'; 	Move-Item -Path C:\go -Destination 'C:\Program Files\Go'; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Tue, 06 Sep 2022 19:35:28 GMT
WORKDIR C:\go
# Tue, 06 Sep 2022 20:12:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 06 Sep 2022 20:12:12 GMT
ENV XCADDY_VERSION=v0.3.0
# Tue, 06 Sep 2022 20:12:13 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 06 Sep 2022 20:12:15 GMT
ENV XCADDY_SKIP_CLEANUP=1
# Tue, 06 Sep 2022 20:12:45 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/xcaddy/releases/download/v0.3.0/xcaddy_0.3.0_windows_amd64.zip"         -OutFile "/xcaddy.zip";     if (!(Get-FileHash -Path /xcaddy.zip -Algorithm SHA512).Hash.ToLower().Equals('63d60531a924a0618a15907a276a67745186a1f92077a48aff2fb68b549b7b80a92238f8a8dca6af82e1840dcdac479e32672b7d62f118c77363be6fae5281a6')) { exit 1; };     Expand-Archive -Path "/xcaddy.zip" -DestinationPath "/" -Force;     Remove-Item "/xcaddy.zip" -Force
# Tue, 06 Sep 2022 20:12:46 GMT
WORKDIR C:\
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f89a6a7fe48246bae14c787b3f68ad97b9d649ad0f0ebc9d654eefa90a681bc4`  
		Last Modified: Wed, 10 Aug 2022 13:24:02 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:700d78f1a37edaf812b6b377963b4ad46402a067ea09535d282788b017da5ce1`  
		Last Modified: Wed, 10 Aug 2022 13:24:00 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97de872a1f90401514b1fd4224785cb2d6301b849142a6612abe22f91f6bef42`  
		Last Modified: Wed, 10 Aug 2022 13:23:58 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89af222c4e6bc5d4bc31acd2d1cf98a0258bcacf3d9a8ecd43f1705eac313351`  
		Last Modified: Wed, 10 Aug 2022 13:23:57 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84a406a2386e04b60cf969f8eb5872e6749e87b083a11e09bf35dc23634c489`  
		Last Modified: Wed, 10 Aug 2022 13:24:05 GMT  
		Size: 25.7 MB (25713776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3810a29e3add75397336456fd6d35a417140bcfa4ba740025ae5377ffd17b83b`  
		Last Modified: Wed, 10 Aug 2022 13:23:55 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d8ff3f35e00b20d78e9808298cedaf198a5e5733be3735faa63d2784a0c5848`  
		Last Modified: Wed, 10 Aug 2022 13:23:56 GMT  
		Size: 558.2 KB (558170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd2ee5093a5c822d5f44ddd45359e9f4b4c3e6dd9c34972e632d74841f81fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.4 KB (1411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e52a0db1305c48db78b1417cb67ba2e8677a7b3493f4c01143a731fa9712fc9`  
		Last Modified: Tue, 06 Sep 2022 19:52:41 GMT  
		Size: 149.9 MB (149895643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a59c3c05e4fcec3faa1d65ef013bc97e2f831d0570db26f58c5fda66b5a8f7e`  
		Last Modified: Tue, 06 Sep 2022 19:52:05 GMT  
		Size: 1.5 KB (1537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9d0b92e053d3cce8a090a1a383b44271c07dece64e96dc9cf467758cc8c56c`  
		Last Modified: Tue, 06 Sep 2022 20:13:30 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ef9a1c5ef13d9a22457d28aa395948c469819ce88e990a637cb238e15a2cde`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86a6269add1abbcb1b0ff1103618d72a08f925461b528a6128245c35d381e67`  
		Last Modified: Tue, 06 Sep 2022 20:13:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5025b5955b1830e84916b28695049d3d61f3e05492fbaf8a471fdcd4977ad070`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2c2aab23d834f4bd6cb85ee8b93d72ad562d73fd7b0b23504f9d32fcbf9efa`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.9 MB (1942308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c13f66dfde8ff4709dbc032e5cdb6cc3bb71b154b513674890d92118b449b`  
		Last Modified: Tue, 06 Sep 2022 20:13:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:latest`

```console
$ docker pull caddy@sha256:740c1c9e461ea1f8a54d7512b35cd31927c814c86455f71e7e8e0c2b6ee423a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:latest` - linux; amd64

```console
$ docker pull caddy@sha256:710992e6e6b73e93f20b620991f7ad024ea43772a899cfef30380bb9802233bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (17033438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:743ed904eb393b6d33d22912502e905e4b46e1685fb61d94a4a60c90bf238bf4`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 02:25:55 GMT
RUN apk add --no-cache ca-certificates mailcap
# Wed, 10 Aug 2022 02:25:57 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Wed, 10 Aug 2022 02:25:57 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 02:25:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Wed, 10 Aug 2022 02:26:00 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_CONFIG_HOME=/config
# Wed, 10 Aug 2022 02:26:00 GMT
ENV XDG_DATA_HOME=/data
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 02:26:00 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 02:26:01 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 80
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 443
# Wed, 10 Aug 2022 02:26:01 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 02:26:01 GMT
WORKDIR /srv
# Wed, 10 Aug 2022 02:26:01 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0c7d01ba8a98bee02450f9f44e2eac5030b38a232f4af1d7c6e816d8230364`  
		Last Modified: Wed, 10 Aug 2022 02:26:26 GMT  
		Size: 304.5 KB (304508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184e55d8db538eb3141ae5d8f19dde0db8ff5646207475523e6417b67fa54425`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 5.8 KB (5831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfd93fd8895ed16c26b3ad309a9254bde758222d5a92ba940ba5158e42abc95`  
		Last Modified: Wed, 10 Aug 2022 02:26:28 GMT  
		Size: 13.9 MB (13916892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbe6c9e2d18a8397350e2e5e7be32a95f7db64805bd36d40c4af25296b6aa6`  
		Last Modified: Wed, 10 Aug 2022 02:26:25 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v6

```console
$ docker pull caddy@sha256:4ce5f3d006a285568a745d0f4158fc7c78c120313960a1cee2b13ff5a1e5152a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.3 MB (16288590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32346edccb2df8c958ba63a08d877c5880a32425fb5e2f96c2c671fe7caf40cd`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 11 Aug 2022 00:57:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Thu, 11 Aug 2022 00:57:54 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Thu, 11 Aug 2022 00:57:54 GMT
ENV CADDY_VERSION=v2.5.2
# Thu, 11 Aug 2022 00:57:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Thu, 11 Aug 2022 00:57:56 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_CONFIG_HOME=/config
# Thu, 11 Aug 2022 00:57:57 GMT
ENV XDG_DATA_HOME=/data
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.title=Caddy
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Thu, 11 Aug 2022 00:57:57 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Thu, 11 Aug 2022 00:57:57 GMT
EXPOSE 80
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 443
# Thu, 11 Aug 2022 00:57:58 GMT
EXPOSE 2019
# Thu, 11 Aug 2022 00:57:58 GMT
WORKDIR /srv
# Thu, 11 Aug 2022 00:57:58 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6663e6bea3ccdb33d6fc98a999afe44c76760f02da1371d023f9974e0c3e906f`  
		Last Modified: Thu, 11 Aug 2022 00:58:42 GMT  
		Size: 304.5 KB (304470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba06166b4d824c7a7dd5fdaf8aa07cff5324044d800e36007991b16f833ae8b`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 5.8 KB (5829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:608b15aea9609795f568dd3f0334c19ce4e4fef22063fd251353ac5633c1fb49`  
		Last Modified: Thu, 11 Aug 2022 00:58:44 GMT  
		Size: 13.4 MB (13364174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef1acfa2e37fe4aa97f742b7cd57630e1c40a92bea0ccde2ba0baaaa175e4a25`  
		Last Modified: Thu, 11 Aug 2022 00:58:41 GMT  
		Size: 152.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm variant v7

```console
$ docker pull caddy@sha256:980e9f462eee7a087aa262df7c59289cadc189060b5c9d5bd4ba6f5bf0c74229
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.1 MB (16074411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c5dd1b61e629ea324876f6a8e52a369f7690d4d0c156f13e7959338e456b3b8`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 17:38:03 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 17:38:04 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 17:38:04 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 17:38:07 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 17:38:08 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 17:38:08 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 17:38:08 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 17:38:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 80
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 443
# Tue, 09 Aug 2022 17:38:09 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 17:38:09 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 17:38:09 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a152bedd5e8d32263f18ecbb89c23375b9f8ff9de1f90018eb566f96d2fff82`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 303.6 KB (303607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af139d15b005159bcdde44df64eff617b34ba1611c67bedc740bd59c0eca563`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3c3ea87c04a2baa15fec00d92b71ab100e02ba4f48ad59985b92dd61c11524`  
		Last Modified: Tue, 09 Aug 2022 17:38:52 GMT  
		Size: 13.3 MB (13347756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bcfe8f96baeba662c26746cab98fae41f81fbc694fb9f62efa260a82ea4927`  
		Last Modified: Tue, 09 Aug 2022 17:38:50 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; arm64 variant v8

```console
$ docker pull caddy@sha256:f0a1658deb0cebfeb8d7fe8c239240c1f6481e159a868d065f83e75fe7423faf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.7 MB (15747027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:74559eb4a47283b65dda99bf1d258f4d6c6c3e16aa70eb68bf7dcdef174c01a7`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:20:53 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:20:55 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:20:56 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:20:59 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:20:59 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:21:00 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:21:01 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:21:02 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:21:03 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:21:04 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:21:05 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:21:06 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:21:07 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:21:08 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:21:09 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:21:10 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:21:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:21:12 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:21:13 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:21:14 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3baea3c3431660a1c20a2c9648914cc3b5c3bbbcde4e05a678a4b48033bd12`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 304.3 KB (304299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f196f799aa76056c71d2afcdceb8f201428a6414a77c19e2690acc6b6f6988d`  
		Last Modified: Tue, 09 Aug 2022 18:21:50 GMT  
		Size: 5.8 KB (5750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba74d0141bf051d97aa61935f807fedf17533fdbc3a5eb08ac0ee1c98c8648b`  
		Last Modified: Tue, 09 Aug 2022 18:21:52 GMT  
		Size: 12.7 MB (12729161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4cb521865ac8487439b62e9f1706da781874a29fe38a9aba5b376b968e4c120`  
		Last Modified: Tue, 09 Aug 2022 18:21:49 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; ppc64le

```console
$ docker pull caddy@sha256:bf7667d542a7f55a0f6c6f0f8a523c944f34bbf661068697e61dc23672573bc2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.4 MB (15425336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdc24d4466b7ad1dc55d7eff8335992e5031fe433446a2fe6470133606dedfae`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:00:50 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:00:52 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:00:52 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:00:56 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:00:58 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:00:58 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:00:59 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:01:00 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:01:01 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:01:02 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:01:03 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:01:04 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:01:04 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:01:05 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d130c379cf611096c8b251962793f03fb6b19d393f7488871a0731fc026264b0`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 306.5 KB (306509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78df06f4f1ddcab0c1a0a3c315fd94c5b6574d58fa3eec8616d7f3fb75c6f8d1`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 5.8 KB (5830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da367b908cafa68846ec3a4c8b9660b96a6901e3d16e3595b5f1e56caa8c1fd`  
		Last Modified: Tue, 09 Aug 2022 18:01:49 GMT  
		Size: 12.3 MB (12309522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a906ddd96d31e91eedb99d93eb0fb5609cf655ad3cc03c6a885f8a9da37d629d`  
		Last Modified: Tue, 09 Aug 2022 18:01:46 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - linux; s390x

```console
$ docker pull caddy@sha256:bb10dd6ab6ab4e01320b6fdb037c4a4c28dafadffb1348a03b240164034cb99f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.4 MB (16362019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:933df8c88011db8f5ddce6060398445ea8b3139efe974c45d3a811acddf8731f`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:15:05 GMT
RUN apk add --no-cache ca-certificates mailcap
# Tue, 09 Aug 2022 18:15:06 GMT
RUN set -eux; 	mkdir -p 		/config/caddy 		/data/caddy 		/etc/caddy 		/usr/share/caddy 	; 	wget -O /etc/caddy/Caddyfile "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"; 	wget -O /usr/share/caddy/index.html "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"
# Tue, 09 Aug 2022 18:15:06 GMT
ENV CADDY_VERSION=v2.5.2
# Tue, 09 Aug 2022 18:15:08 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64)  binArch='amd64'; checksum='b19eb832e341f7bdb1c6fec2333564745a38f9aa814a14e7843a1b20468e0cdc6547977d3ae5a63d687dd7b9a68f90792e228020bf2481f916d9982322361632' ;; 		armhf)   binArch='armv6'; checksum='de401bdf04f67647df89439292726c3a37d833edd7313a72fe47d45aa18c93aa6ef5b8718ffc8accb70cd356c0e62fc1a18808cd4e2de2357e80d44aef168d19' ;; 		armv7)   binArch='armv7'; checksum='3fda191727748eb23805e0e765b5794333a31c265879d7d54af6ddaa94cef14534c8ea993a231cbf94855c388a9c9a613be64260e2a8add6cc8ae230c218c59e' ;; 		aarch64) binArch='arm64'; checksum='b71a6c7961b4b7acda6ec71b70db2e8695572196a283a56eb910d3da08867e6f298c6cf34c12ebc35235f3de3bc833109596b56a3560b03ca1c3bcdb53b59372' ;; 		ppc64el|ppc64le) binArch='ppc64le'; checksum='5c98c82b64dab878fdbd158d7b162c2bdb36ea9606b1c06b0c04ee2060e6a42f169c876c70eb3558acd37e25395c3ed1764c5753ede79a9e05dbf03cef69d410' ;; 		s390x)   binArch='s390x'; checksum='7c86521e8d3e75899f91106863e46a43be3cd76b5ae63be81e735ad849182b0c08a98b7f8cdd3d975aed9b4e741ed02b42fa8435ca95d893bb00850a53b78a5c' ;; 		*) echo >&2 "error: unsupported architecture ($apkArch)"; exit 1 ;;	esac; 	wget -O /tmp/caddy.tar.gz "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_linux_${binArch}.tar.gz"; 	echo "$checksum  /tmp/caddy.tar.gz" | sha512sum -c; 	tar x -z -f /tmp/caddy.tar.gz -C /usr/bin caddy; 	rm -f /tmp/caddy.tar.gz; 	chmod +x /usr/bin/caddy; 	caddy version
# Tue, 09 Aug 2022 18:15:09 GMT
RUN [ ! -e /etc/nsswitch.conf ] && echo 'hosts: files dns' > /etc/nsswitch.conf
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_CONFIG_HOME=/config
# Tue, 09 Aug 2022 18:15:10 GMT
ENV XDG_DATA_HOME=/data
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.title=Caddy
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Tue, 09 Aug 2022 18:15:10 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Tue, 09 Aug 2022 18:15:11 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 80
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 443
# Tue, 09 Aug 2022 18:15:11 GMT
EXPOSE 2019
# Tue, 09 Aug 2022 18:15:11 GMT
WORKDIR /srv
# Tue, 09 Aug 2022 18:15:11 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75905bff4d3de6daed73e1c8f83d37ce44f2a30ebc2a9764fb82f89c1344ac7e`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 304.7 KB (304742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352ba655d1c5ab97f65a61931fb410d5dbb71a2aa01bf2c610156fb2c4f76fce`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 5.8 KB (5827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4337a42e49a276ba328d45c8af4bbc1b56c3c67edc730259d1d218a31e263ce`  
		Last Modified: Tue, 09 Aug 2022 18:15:55 GMT  
		Size: 13.5 MB (13460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73809ed76eaa5655558127e091c5a214118515f72d7c9e085c171a7cc64ae1dd`  
		Last Modified: Tue, 09 Aug 2022 18:15:53 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:latest` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore`

```console
$ docker pull caddy@sha256:d98344a194f90621248b3c94ba8b3c2fe4cbc4ee05cfc22334d2a747cb2350bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.17763.3287; amd64
	-	windows version 10.0.20348.887; amd64

### `caddy:windowsservercore` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `caddy:windowsservercore` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-1809`

```console
$ docker pull caddy@sha256:0390ac5f55f7a6eae2a40f9256802bc1c6bbe33a01f41ed73b0d932c91f76f04
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `caddy:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull caddy@sha256:9cdcee9e568f42fc02437c2a617ffe6f781bd274d307e2578370ae8424114582
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2692631679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdd24525e4c506b89eb6faf38a96e9523c6e21233f08d077458802a62c1028b`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:06:10 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:06:10 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:07:14 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:07:15 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:07:16 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:07:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:07:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:07:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:07:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:07:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:07:21 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:07:22 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:07:23 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:07:24 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:07:25 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:07:26 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:08:15 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:08:16 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de895f61ee42c0f5dacbf0e50b46c4c9c2bc2216e1fe588c3bd77150d9aaccc`  
		Last Modified: Wed, 10 Aug 2022 18:11:11 GMT  
		Size: 357.6 KB (357571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677ef98f58f5ba429a7fee0ca5739cefc455653ed9f48184dc448c7632f5f517`  
		Last Modified: Wed, 10 Aug 2022 18:11:10 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d949c2b3da955c1b31a95737a730837726c825eaf149f5a0fcf2c19b30befb`  
		Last Modified: Wed, 10 Aug 2022 18:11:13 GMT  
		Size: 14.2 MB (14243229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7883b40c7ce64ab1b3f2863a652d80e2a804e22c068ef017a7da4d045280e3a9`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ce2e999a8e0415e61518e939ab6bad5065244caf150d0c0b9b57921d2d6fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e9b06f668970f774120eeaf4dff90afcb4ced5f0866fb091e935b5d88ede88`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7e02681340631e2f8b5113c621884401f9c85827a4cddc07573f70ae50f555`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ca95f9ca59786ae463015e0f57c8837513afb3d4d8dc24f211e3062d86fb1e`  
		Last Modified: Wed, 10 Aug 2022 18:11:08 GMT  
		Size: 1.4 KB (1380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5296e7682c77aaadaeaea56a389d49c99a9710032773ced8ae13c0c5b335fb5`  
		Last Modified: Wed, 10 Aug 2022 18:11:06 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88eb043066ea67cd3c1d0992598fee14402e890c9eddb09a62da88c42b389882`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c20e94b473f771b38694b861071536512098e7aadb4268ea365603b3a1097de`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe5e25e82fff1a8a871c2d8b4f34cdaa896fb77df4cf62656bfde514db6796c`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349b4e90a9af566bbbba422dec3d130cc35d1dc72025623bee07ceee1e3087c6`  
		Last Modified: Wed, 10 Aug 2022 18:11:05 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01b44eb195800b31056b46337470e577d43d591d5c9a721495f1f3689df1e24`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d285ab47afe7667516ab8ad27b7b32ba6770178cbfa051554de786f0f6de9211`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8149d8d4aa5ca20f53b61b456f01c772296cd4841caf76091d6e841c3293737`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5532f76a6bebfe8f153e1f291505e604b3056dd019f1eadb4c890dc04ce95cd`  
		Last Modified: Wed, 10 Aug 2022 18:11:04 GMT  
		Size: 295.6 KB (295620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e247074218115dfed4d7a054479a7c5e030287eae6180ed57d0f1c83ae97fc5e`  
		Last Modified: Wed, 10 Aug 2022 18:11:03 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `caddy:windowsservercore-ltsc2022`

```console
$ docker pull caddy@sha256:ce2b42e067d32df033d35738362e9279cbb832f91d400e14a9dd2c5d2e50c1eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `caddy:windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull caddy@sha256:517a012afe83a576b0478b2c131f5c63a0bd72fe746bc611ef304f1e84dc3323
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2332378364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b0c35bf0a951ae3c33c437ddae6c410aa8ee5502f4cfcf578cbfcca953a3599`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 18:08:47 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/979e498d6d01e1fe7c22db848a3e3bc65369183f/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 10 Aug 2022 18:08:48 GMT
ENV CADDY_VERSION=v2.5.2
# Wed, 10 Aug 2022 18:09:13 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.5.2/caddy_2.5.2_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('b104d364a458f457bab24f12f97470612035f705fceb170ce16b567e18e0429a18a726f6b1bb435f92d28a659aee52c08c0bac3be41b7f23887b8e7307507482')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 10 Aug 2022 18:09:14 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 10 Aug 2022 18:09:15 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 10 Aug 2022 18:09:16 GMT
LABEL org.opencontainers.image.version=v2.5.2
# Wed, 10 Aug 2022 18:09:17 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 10 Aug 2022 18:09:18 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 10 Aug 2022 18:09:19 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 10 Aug 2022 18:09:20 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 10 Aug 2022 18:09:21 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 10 Aug 2022 18:09:22 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 10 Aug 2022 18:09:23 GMT
EXPOSE 80
# Wed, 10 Aug 2022 18:09:24 GMT
EXPOSE 443
# Wed, 10 Aug 2022 18:09:25 GMT
EXPOSE 2019
# Wed, 10 Aug 2022 18:09:44 GMT
RUN caddy version
# Wed, 10 Aug 2022 18:09:45 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ec5da9dac23bde972af7de24ce482fbe81d8aefd00974283db7bf7329bc627`  
		Last Modified: Wed, 10 Aug 2022 18:11:35 GMT  
		Size: 633.5 KB (633527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7115307387c87323f3d4ece589183771a112092cee1ce228d8d5115cd5f81161`  
		Last Modified: Wed, 10 Aug 2022 18:11:34 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd7443b36f536075714d920a7edc69342540875be613780fa39acd4578dbcc35`  
		Last Modified: Wed, 10 Aug 2022 18:11:37 GMT  
		Size: 14.5 MB (14483236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1c5c734982c03071a686a8dde06eea8caa8225b97b7475724e1992ab83c095`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852db0c5e3cd48a5d3359f7bbd815bbafaa141bb4f7b7fd584805940fc0a9838`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60989074a8d5a939f7e0dc297cc95a1ac89ffb64d3960688d2212cf428ea788d`  
		Last Modified: Wed, 10 Aug 2022 18:11:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a59c476dbb6450af97f698281a36593e1517533c6560095a3794240d26e4a61`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101d92d75032c54e3fb9e78b433b377a3ab5f19c3ec8071325b7ac5f8d8fb496`  
		Last Modified: Wed, 10 Aug 2022 18:11:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846b98eee44b08c1ab571f0740ac9f07e7189875539f5f16f0f9ff20c9158260`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe96e9bb12efddf416f88596ac877e248ef65ae462899a41ff1bdcc559951796`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdf939a2e5078185de0aa0fb9b989891ecf54876c468bf845e727b5add5555e`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd4a929572d26c0fa4860f0e5520bdd46024fd6baa76751c3fc6d77d321effe`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef4c866a2e92e6eb2dd8cb543c359e7f3a71b03f3e1daf718fadbdad46f1480f`  
		Last Modified: Wed, 10 Aug 2022 18:11:29 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1913390b80af8b994c1aa5cdcc9589b5f3bd28b9aadf3404deee1c92b286f64`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac02dbbe3aec3978131e958bc6c9a93fbb18f4116816697e6b7ba99dd355dbd`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0dac1a6a7b4421ff2121d3ed185cb87ad1d518b910cd07ba26604c179c4cb0`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7ccb5803eeac5ac1d753bb79eb4da4b22f1e6f7728cd2cf22317ab549c7a5f`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 349.8 KB (349824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddae6180de77f50cfed8829ad06d23a1d5693a99a543583d49a3446433da6ba6`  
		Last Modified: Wed, 10 Aug 2022 18:11:27 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
